# Basic GIS

## Geographic coordinate system

- **Latitude**: North-South [-90, 90]
- **Longitude**: East-West [-180, 180]
  - aka Meridian
  - 0 degree is Greenwich, England (Prime Meridian)
- Format
  - Degree Minute Second (DMS) ex. 10° 15' 15" N
  - (S->M) Degree Minutes Decimal (DMD) ex. 10.15.25° N
  - (M->D) Degree Decimal (DD) ex. 10.2542° N
  - Radian ex. 0.178960 rad

## Geodetic datum

Global datum reference or reference frame

- for precisely representing the position of locations on Earth
- or other planetary bodies by means of geodetic coordinates.

- **WGS 84** (World Geodetic System 1984)
horizontal datum intended for global use,
whereas Earth's surface is approximated by an ellipsoid.
Datum can be **TRANSFORM** with the followed methodwith the followed method :

  - Helmert transformation
  - Molodensky-Badekas transformation
  - Molodensky transformation
  - Grid-based method

## Bearing and Distance

```python
from math import pi, sin, cos, atan2, sart

__RADIAN__ = pi/180
__RADIUS__ = 6371.01 * 0.539957

def getSphereRelationReference(lon1, lat1, lon2, lat2):
    lon1 = lon1 * __RADIAN__
    lat1 = lat1 * __RADIAN__
    lon2 = lon2 * __RADIAN__
    lat2 = lat2 * __RADIAN__

    # Delta
    dlon = lon2 - lon1
    dlat = lat2 - lat1

    # Distance
    '''
    a: square of half the chord length between the points
    c: angular distance in radians on the sphere
    x: angular distance in radians from the first point to the second point
    y: initial bearing in radians (clockwise from north)
    '''
    a = sin(dlat/2)**2 + cos(lat1) * cos(lat2) * sin(dlon/2)**2
    c = 2 * atan2(sqrt(a), sqrt(1-a))
    y = sin(dlon) * cos(lat2)
    x = cos(lat1) * sin(lat2) - sin(lat1) * cos(lat2) * cos(dlon)
    
    return {
        'distance': __RADIUS__ * c,
        'bearing': atan2(y, x) / __RADIAN__
    }
```

## Rhumb Line vs Great Circle

- **Rhumb Line**: Constant bearing
- **Great Circle**: Shortest distance

> - **Great Circle** is the **shortest distance** between two points on the surface of a sphere, which always lies on a plane that passes through the center of the sphere.
> - **Rhumb Line** is a curve on a sphere that crosses all meridians at the same angle, that is, a path with constant bearing as measured relative to true or magnetic north.

## Type of Geometric Data

- **Point**: 0 dimension, position
- **Multi Point**: 0 dimension, Group of buoys
- **Line**: 1 dimension, Road, River, etc.
- **Multi Line**: 1 dimension, Group of roads
- **Polygon**: 2 dimension, Area, Country, etc.
- **Multi Polygon**: 2 dimension, Group of countries

## Challenge of GIS DB

- Geometric (spatial) operation
  - Search in given area
  - Containing/Convex hull
  - Clustering
  - Nearest point search
  - Distance calculation
  - Centroid calculation
  - Minimum Border Rectangle(MBR)/Boundary
  - Union, Intersection and other polygon modification
  - etc.
- Volume : Especially positioning data (time series)
  - Navigation radar: 50 tracks/sec = 4.3M tracks/day
  - Air Surveillance radar: 1000 tracks/sec = 86.4M tracks/day
- Time critical/causality
  - query latency
  - network latency
  - concurrent access
  - r/w ratio

### RDBMS with GIS

- **PostGIS** (PostgreSQL) open source
  - Most advanced and performant (claimed)
  - full featured and widely used
- MySQL (free)
  - limited spatial function but on improvement
  - stability issue
- MS SQL Server (commercial)
  - limited spatial function
  - performance issue
- Oracle Spatial (commercial)
  - full featured + widely used

#### Why not RDBMS?

- designed for Read over Write
  - defense: R/W balanced
- ACID compliance
  - defense: not required
- not full till time critical
- not scale well

#### Other DB options

- In-memory DB
  - Redis
  - Memcached
- Event/Time series DB
  - InfluxDB
  - TimescaleDB
- Limit the capability
  - No transaction
  - No history tracking
  - No spatial operation

#### XpeedDB : Specialized DB

XpeedDB is a specialized DB for GIS data.

## How non-GIS data can be retrieved?

### Tree

- **B-Tree** (Balanced Tree)
  - **B+Tree** (Balanced Tree)
    - **R-Tree** (R-Tree)
      - **R+Tree** (R+Tree)
        - **R*Tree** (R*Tree)

### K-D Tree

- **K-D Tree** (K-Dimensional Tree)
- **K-D Tree** is a space-partitioning data structure for organizing points in a k-dimensional space.

### R Tree

- **R-Tree** (R-Tree)
- **R-Tree** is a tree data structure used for spatial access methods, i.e., for indexing multi-dimensional information such as geographical coordinates, rectangles or polygons.

### Minimum Bounding Rectangle (MBR)

- This method, known as the Rotating Calipers approach, 
- It is based on the idea that a side of the smallest 
  area bounding box aligns with a side of the polygon. 

### Polygon Containing

1. Draw a horizontal line to the right of each point, to infinity
2. Count the number of times the line intersects with polygon edges.
3. inside===odd or point lies on an edge of polygon.   outside===even

### Nearest Neighbor Search

### Closest Point of Approach (CPA)

- **CPA** (Closest Point of Approach)
- **CPA** is the minimum distance between two moving objects at a given time.
- **CPA** is used to determine the risk of collision between two objects.

### Centroid of Polygon

```C#
public static Point GetCentroid(List<Point> points)
{
    double x = 0;
    double y = 0;
    double area = 0;
    int i, j, n = points.Count;

    for (i = 0; i < n; i++)
    {
        j = (i + 1) % n;
        area += points[i].X * points[j].Y;
        area -= points[i].Y * points[j].X;
    }
    area /= 2;

    for (i = 0; i < n; i++)
    {
        j = (i + 1) % n;
        x += (points[i].X + points[j].X) * (points[i].X * points[j].Y - points[j].X * points[i].Y);
        y += (points[i].Y + points[j].Y) * (points[i].X * points[j].Y - points[j].X * points[i].Y);
    }

    x /= (6 * area);
    y /= (6 * area);

    return new Point(x, y);
}
```
