# Introduction to Defense Technology

## What is State?

State is a **political unit** without unified definition. The definition by *Max Weber* is the
most commonly used :
> State is a **compulsory** political organization with a **centralized government** that maintains a **monopoly of the legitimate use of force** within a certain **territory**.
\
\
> *Compulsory* = required by law or a rule

From *Weber*, it can be interpreted that a state must at least be consisted of

- Population
- Territory
- State Power
- Government

## What is War?

> War is the continuation of policy with other means.
> \
> -- *Carl von Clausewitz*

### Trinity of War

- **People** Hate, Enmity, Primal Violence, Passion
- **Government** Politics, Reason, Intelligence
- **Military** Calculations, Game of Chance, Odds, Value

### Fog of War

The fog of war (German: "Nebel des Krieges") 

- the **uncertainty in situational awareness**
- experienced by participants in military operations

## Technology as Decisive Tool

- **Roman Empire Battle Formation**: Tortoise Formation
- **Viking Battle Formation**: Shield Wall
- **British Long Bow**:
- **Mongolian Horse Bow**:
- **Chinese Wall**:
- **Samurai Equipment**: Katana, Yumi, Yari, Naginata, etc.
- **Gun Powder & Germ against Aztec**:
- **WW II : German Tank**:
- **WW II : German U-Boot**:
- **WW II : Enigma**:
- **WW II : Montgomery vs Rommel**:
- **Ukrainian Drone vs Russian Tank**:

## What are the factors to win a war?

### Find Black Cats in a Dark Black Room

The concept of **Find Black Cats in a Dark Black Room** is a metaphor for the difficulty of finding something that is not there. It is often used to describe the difficulty of proving that something does not exist.

### Staff Grouping

- **J-1**: Personnel/HR
- **J-2**: Intelligence
- **J-3**: Operations
- **J-4**: Logistics
- **J-5**: (Future) Plans
- **J-6**: Communications & IT
- **J-7**: Civil Affairs

### Level of Military Operation

- **Strategic**: National Level
- **Operational**: Theater Level
- **Tactical**: Battlefield Level

## Network Centric Warfare

**NCW** is a military doctrine or theory of war pioneered by the United States Department of Defense in the 1990s. It seeks to translate an information advantage, enabled in part by information technology, into a competitive advantage through the robust computer networking of well informed geographically dispersed forces.

Layer of NCW

- **Sensor Layer**: Collecting information
- **Info-C2 Layer**: Processing information
- **Effector Layer**: Acting on information

### NCW vs CMS

|Criteria|CMS|NCW|
|---|---|---|
|**Focus**|Battlefield|Theater|
|**Level**|Tactical|Operational|
|**Time**|Real Time|*Near* Real Time|
|**Coverage**|Mission area ~15nm and/or between missions|All area of operation|
|**Weapon**|Kinetic|Kinetic & Non-Kinetic|
|**Separation**|Warfare dimension (SuW, AAW, ASW)|Staff function (J-1...7)|
---

- SuW: Surface Warfare
- AAW: Anti-Air Warfare
- ASW: Anti-Submarine Warfare

### NCW Capabilities

- **Situational Awareness**: Common Operational Picture (COP)
- *Share situational picture between units*
- Plan, Execute, Assess (PEA)
- **C2** (Command & Control)
  - Head Quarter (HQ) -> Area of Operation (AoO)
  - HQ/AoO -> Supporting Units
  - AoO -> Surveilled Units
  - AoO -> Ships, Aircrafts, etc. aka Ship
  - Ship -> Ship
- Resource pooling and distribution (sensor, weapon, etc.)

#### Surveillance Station

- **Featured with sensors**
  - Radar
  - EO/IR (Electro-Optical/Infrared)
- 24/7 operation
- Task
  - Processing: Detect, Track, Classify, Identify
  - Filtering: Noise, Clutter, False Alarm
  - Distribution: Share to other units
- Built at choke point 
  
> choke point is a strategic narrow route providing passage through or to another region

# Situation Awareness & Combat Management

## timeline

- Ancient Battle... How could you know, what is happening?
> At least, you know, where are your enemies. LOL
- **Direct Confrontation in WW-I**
  - cute explanation:
  - pros: you can see your enemies
  - cons: you can see your enemies
- **Hide & Seek started in WW-II**
  - cute explanation:
  - pros: you can hide from your enemies
  - cons: your enemies can hide from you
- **The Real Hide & Seek is at Sea**
  - cute explanation:
  - pros:
  - cons:
- **More Hide & Seek with Invention of Radar** 
  - cute explanation:
  - pros:
  - cons:
- Today : **Pure Hide & Seek**

## From past to present : **Sand Table**

Model of terrain, battlefield, etc. to visualize the situation and plan the strategy.

## What is Situation Awareness? ***SA***

A tool for observation of the situation in the battle field.

- To understand the situation
- To predict the situation
- To decide the strategy

Tool for all type of military operation

> OODA Loop (Observe, Orient, Decide, Act)

- SA != Computer system
- SA provide
  - Accurate information
  - Overview + Detail
  - Real time + Near real time
  - Standardized information
- Computer system provide better SA

## How can we get the information?

> Information Pyramid (from bottom to top)
> \
> *Wisdom > Knowledge > Information > Data*

### Source of Data/Information/Intelligence

|Source|Characteristics|Input|
|---|---|---|
|**Sensor**|Automatic detection, Processable output, Objective, Additional processing is required|Synchronized and Automatically|
|**Human observation**|Subjective, Additional direct consumable, Low rate of update|Manually|
|**Survey**|Objective, Low rate of update, Base of everything else|Stored in database|
|**Intelligence**|Direct consumable, High value|Manually and/or exchange with other system|

### Quality of Data Source

- **Detection**: Knowing existence and/or position of track
- **Classification**: Knowing class, type of track
- **Identification**: Knowing adversity, identity of track. Track can be identified mostly
with optical contact or electrical footprint.

> Weapon: used for identified target ONLY

## Minimizing the Observation Time

### Map Display: Land

> Land map has no widely used standard.

- **S57 & S63 : Nautical Chart**: for sea
  - S57: data format
  - S63: data protection
- **Air Control** : Map Detail is not important. Only the position of aircraft is important.

> Is 3D a Good Map Display?
> \
> 3D is not a good map display. It is good for visualization, but not for information.

- **Additional Military Layer (AML)**
  - Operation picture (Mid-Std 2525D):
  - Geographic Reference (Point, Line, Polygon, etc.)
  - Other addon
  - Weather
  - Construction
  - Walkway, road, river and other vector lines
  - Digital Surface Model (DSM)
  - Digital Terrain Model (DTM)

## Track vs. Target

- **Target**: Object or unit in interest
- **Track**: Tracked information received from data source
  - Automatic data fusion/correction by machine
  - Further processing by operator is required
    - Related information
    - Classification and identification
    - Final decision
  - History of track is desired
- Goal: Track => Target (accurate and in time)

### Track Identity

- pending: track is not identified
- unknown: track is identified, but not classified
- assumed friend
- friend
- neutral
- suspect or joker:
- hostile or faker (for exercise)

> MILSTD-2525 : Military Symbol Standard

## Combat Management System (CMS)

- Integrated computer system for force unit management in **tactical** level
  - Situation awareness
  - Communication
  - Weapon control
  - C2
  - etc.
- Widely used in NAVY
- Brain & Heart of the ship
- Enhance tempo of OO-DA Loop

### History of CMS

- CIC (Combat Information Center) Room: Old school
- CIC Room : Upgraded
- CIC Room : Modern
- Modern CMS

#### Multi Function Console (MFC)

- Feature
  - Own ship
    - keyword: display of roll, pitch, heading, speed, etc.
  - Situation Awareness
    - layer: tracks, plots, figures, support graphics, radar, maps
  - Tactical Navigation
  - Air Control
  - EMCON (Emission Control)
  - Sensor Control
  - Combat Operation & Weapon Control
  - Tactical Data Link

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

### Vector DB for Large Language Modelling
---
---
# Map Engine

## Map

A map is a **symbolic depiction** emphasizing **relationships** between **elements** of some
space, such as objects, regions, or themes.

> In our case, a map is the depiction of relationships between GIS data on the given material

### Map Characteristic

#### Orientation

- Depending on the map application
- This characteristic is essential for the map on paper but less important for the electronic map.

ex. Map of Utrecht, Netherlands (1695) is canal oriented map.

#### Scale and Accuracy

- Map on paper must inform about the scale of the map in ratio so that the user can
estimate the actual size of the elements depicted in the map.
- Map with lower scale
emphasizes the details and accuracy, the higher scale the overview.

ex.

- ENC TH045 : The standard overview map for Thai Gulf and Andaman Sea.
- ENC TH0011030 : Detail map for Phuket habour.

- The important characteristic of the map scale is the correctness and the consistency of
the distance between different elements in the map. To be pendant, no map can
provide these due to the map projection. But the accuracy should be acceptable.

- **Scale on Electronic Map** 
  - In normal case, map scale cannot given due to different DPI of monitor
  - For navigation system like ECDIS or WECDIS :
    - Monitor must have the given DPI and be certified.
    - Map scale can be given.
  - Map can be zoomed-in and zoom-out.
  - The resolution depends on the GIS data (point distance)

### Map and State Sovereign (อาณาเขต)

Without given coordination (lat/long) according to the law, no information about
sovereign should not shown in the map. Because no map scale can fit the description.
> อย่าใส่เส้นอาณาเขตมั่วๆซั่วๆ

ex. Sea zone according to the international law (UNCLOS-1982).

### Symbology and Design

- Declare the existence of geographic phenomena
- Show location and extent
- Visualize attribute information
- Add to (or detract from) the aesthetic appeal of the map.
- Establish an overall gestalt order to make the map more or less useful.
- **In the military use, symbol on the map should follow the standard.**

### Type and Application

- **Electronic Map**
  - can provide features
  - flexible
  - multi-layer can be over-layed
  - analytical function
- **Paper** Less applicaltion
  - for legal purpose
  - special purpose/survey

## Map Projection

### Type

- Tangent: Tangent to the globe
- Secant: Intersect the globe

- Cylinder: 0
- Cone: (0, 90)
- Plane: 90

### Mercator Projection

- Tangent Cylinder
- Conformal
- Rhumb line is straight line
- **Distortion** at high latitude
- Used for navigation
- Used for ENC (Electronic Navigational Chart)
- Used for Google Map

### Transverse Mercator projection

- ...

### UTM Coordination

- **UTM** (Universal Transverse Mercator)

### UTM Zone

- 60 zones
- 6 degree each
- 84 degree each
- 2 zones for Thailand
  - 47N
  - 48N
  
### UTM vs Latitude/Longitude

- UTM is not a projection
- UTM is a coordinate system
- UTM is a grid system
- UTM is a metric system
- 10 Digits of UTM : 1 = 1sqm, easy for distance calculation.

### Equal Area Projection

need picture

### Gall–Peters projection

need picture

## Electronic Map-Engine

### Raster Map (Google Maps ตอนไม่ซูมเยอะ)

- Raster picture of map or raster information
  - Scanned map from the existing paper
  - Photo (air, satellite) Pre-rendered map (Tile Map, Old Google Map)
  - Elevation of terrain
- Information cannot be extracted.
- Not possible to interact with the map elements.
- Lower processing power
- Ease of use and deployment

### Vector Map (Google Maps ตอนซูมเยอะ)

- GIS information e.g. point, line, polygon
  - Survey intensive for information gathering
  - Each data can contain additional data
- Information can be directly used.
- Good for interaction
- High processing power
- Complex data query from GIS database
- Complex map render and symbol drawing
- Application must be highly optimized.

### Shape File

- **geospatial vector data format** for geographic information
system (GIS) software.
- The shapefile format can spatially describe vector features:
  - points, lines, and polygons, representing,
    - for example, water wells, rivers, and lakes. 
  - Each itemusually has attributes that describe it, such as name or temperature.

### GeoJSON

```json
{
    "type": "Point",
    "coordinates": [102.0, 0.5]
}
```

```json
{
    "type": "Linestring",
    "coordinates": [
        [102.0, 0.0], 
        [103.0, 1.0], 
        [104.0, 0.0]
    ]
}
```

- Open standard format designed for representing simple GIS
- Non-spatial attributes can be included.
- Supported Type: Point, Line, Polygon
- Popular for Web-Application
- Format is neither size nor processing efficient.
- Not recommended for high performance system

### DEM File

- Standard geo-spatial file format
- Grid (raster) based digital elevation model
- Developed by *the United States Geological Survey* (USGS)
- Categorized into 4 levels according to the accuracy

### GeoTIFF

- GeoTIFF is a public domain metadata standard which allows georeferencing information to be embedded within a TIFF file.

### S57 & S63 : Nautical Chart

- S57: data format
- S63: data protection

## Map Engine Reference Point

## Position Transformations

## Tile Map

## Event Handling

- Handle double click event on map for symbol detail
- Handle drag event on map for pan
- Handle scroll event on map for zoom
- etc.

## Map Engine Optimization

|Optimization|CPU||GPU|
|---|---|---|---|
|Canvas rendering|Fetch tiled map and tracks from servicer -> Draw tiled map into offscreen -> Draw tracks into offscreen -> Draw offscreen into onscreen||Render pipelining to monitor|
|WebGL rendering|Fetch tiled map from service -> prepare tiled map to GL|fetch tracks from server -> Prepare tracks to GL|Transform data locations to vertices positions -> Calculate UV from tracks textures -> render to monitor|

> GL : Graphics Library
> \
> UV : Texture Coordinate

# Positioning System

## Nautical Navigation

- It's still used nowadays
- In the critical env, it's obligation for the seaferer
- Method of positioning with pririty
  - Bearing coss cut
  - Radar cross cut
  - Astronomical navigation
  - Electrical/Satellite navigation

### Bearing Cross Cut

- Measurement of bearing from the ship to reference point
- Bearing = angle between line of sight and north
- Precise info of
  - position of reference point on nautical chart
  - The north direction

### Magnetic compass

### Magnetic pole

- Magnetic pole is not the same as geographic pole

### Iso-gonic line

- Iso-gonic line is the line of equal magnetic declination

### Compass rose

- Compass rose is the symbol of magnetic declination

### Ship magnetic compass

### Gyroscopic inertia

- Gyroscopic inertia is the property of a rotating body with respect to its angular momentum.

### Gyrocompass

- Gyrocompass is a compass with a gyroscope that is mounted so that its axis can rotate freely to any orientation.

### Gyroscope in Space

- Gyroscope in space is the property of a rotating body with respect to its angular momentum.

### Electronic Gyrocompass

### Gyro Repeaters

For the ship with multiple bridge (e.g. aircraft carrier), gyro repeaters are used to show the heading of the ship.

### Astronomical Navigation

- Bearing cross cut is limited to coastal area
- For navigation in the open sea, astronomical navigation is used.
- Complex calculation
- High skill of measurement and calculation
- Dependent and reliable precise (600m)

## Distance between sun and earth

- 1 AU (Astronomical Unit) = 149,597,870.7 km
- 1 AU = 8.3 light minutes

### Sextant for Angel & Distance Measurement

How to measure the angle between two objects?

### chronometer watch

### Astronomical Almanac

> Almanac is an annual publication listing a set of events forthcoming in the next year.

astronomical almanac is a book that contains astronomical data, mostly tables, used by astronomers, navigators, and others.

### Star map

### Sun and Moon path

> LOP : Line of Position

# Satellite Positioning System

## GPS (Global Positioning System)

> Number of satellite required 
> \
> 2D : 3
> \
> 3D : 4

### GPS Frequency

|Band|f (MHz)|Description|
|---|---|---|
|**L1**|1575.42|coarse acquisition (C/A) and encrypted precision P(Y) codes, plus the L1 civil (L1C) signal and Military code (M-code) on Block III satellites and beyond|
|**L2**|1227.60|P(Y) code, plus the L2C and M-code on Block IIR-M and newer satellites|
|**L3**|1381.05|used by the Nuclear Detonation (NUDET) Detection System (NDS) payload|
|**L4**|1379.913|being studied for additional ionospheric correction|
|**L5**|1176.45|safety of life (SoL) applications, such as aviation|

### GPS Distance Calculation

- Between satellite and receiver
- d = ct; c is the speed of light

### GPS Position Calculation

> GNSS : Global Navigation Satellite System
