# Basic of Sensor

## Sensor

A device that produces an **output signal** for the purpose of sensing a *physical* phenomenon.

### Example Type of Sensors

- **E/M signal**: antenna, microphone, camera
- **Light** (also E/M): photoresistor, photodiode, phototransistor, Light/Laser
- **Heat** (can be E/M): thermistor, thermocouple, infrared sensor
- **Sound**: microphone, piezoelectric sensor, hydrophone
- **Acceleration** and **Movement**: accelerometer, compass, GPS
- **Phase Acceleration**: gyroscope
- **Pressure**: barometer, piezoelectric sensor, piezoresistive sensor
  - Height measurement
- **Particle detection**: smoke detector, Geiger counter

### Sensor Sensitivity

Indicates how much its **output** changes when the **input** quantity it measures changes.

$\text{sensitivity} = \frac{\Delta \text{output}}{\Delta \text{input}}$

### White Noise

A random signal having equal intensity at *different frequencies*, giving it a constant power spectral density.

> Copilot: A random signal with a *flat power spectral density*.

### Gaussian Distribution

A continuous probability distribution that gives a good description of data that cluster around a mean.

> Q: How gaussian distribution is related to white noise? \
> A: White noise is a random signal with a flat power spectral density, which means the signal has equal power in any band of a given bandwidth. Therefore, the signal has a normal distribution in the time domain.

### Electromagnetic Wave Propagation

### Power vs. Distance

$P = \frac{P_0}{d^2}$

### Noise Floor

The measure of the signal created from the sum of all the noise sources and unwanted signals within a measurement system, where noise is defined as any signal other than the one being monitored.

> **SFDR (Spurious Free Dynamic Range)**: The ratio of the RMS value of the fundamental signal to the RMS sum of all other spectral components.
> **Harmonics**: A harmonic of a wave is a component frequency of the signal that is an integer multiple of the fundamental frequency, i.e. if the fundamental frequency is $f$, the harmonics have frequencies $2f$, $3f$, $4f$, etc.

### Frequency and Wavelength

$wavelength = \frac{speed}{frequency}$

### Standing Wave

A wave that oscillates in time but whose peak amplitude profile does not move in space.

> *Zwei Feste Enden*: Two Fixed Ends
> *Zwei Offene Enden*: Two Open Ends
> *Festes und Offenes Ende*: One Fixed and One Open End
> *Zwei Freie Enden*: Two Free Ends
> *Festes und Freies Ende*: One Fixed and One Free End
> *Zwei Verschiedene Enden*: Two Different Ends
> *Festes und Verschiedenes Ende*: One Fixed and One Different End
> *Zwei Gleiche Enden*: Two Same Ends
> *Festes und Gleiches Ende*: One Fixed and One Same End

### Antenna

A transducer that converts radio frequency fields into alternating current or vice versa.

#### Dipole Antenna

A radio antenna that can be made of a simple wire, with a center-fed driven element.

#### Omni Directional Antenna

An antenna that radiates uniformly in all directions in one plane, with the radiated power decreasing with elevation angle above or below the plane, dropping to zero on the antenna's axis.

#### Directional Antenna

An antenna that radiates or receives greater power in specific directions allowing increased performance and reduced interference from unwanted sources.

> HPBW (Half Power Beam Width): The angle between the half-power (-3 dB) points of the main lobe.

#### Yagi-Uda Directional Antenna

A directional antenna consisting of a driven element (typically a dipole or folded dipole) and additional parasitic elements (usually a single reflector and several directors).

---

# Radar

A radiolocation system that uses radio waves to determine 

- the distance (ranging), 
- angle (azimuth), 
- and radial velocity of objects relative to the site.

- **US Naval Research Laboratory (1930)** is the first to use the term **Radar**.
- **Chain Home Radar, UK (1938)** is the first operational radar system. It is used to detect aircraft and ships by transmitting a pulse of radio waves and detecting any reflected pulses.

## Radar Principle

## Radar Frequency Band

| Band | Frequency | Wavelength range | Notes |
| ---- | --------- | ---------------- | ----- |
| HF | 3-30 MHz | 10-100 m | Coastal radar systems, over-the-horizon (OTH) radars; 'high frequency' |
| VHF | 30-300 MHz | 1-10 m | Very long range, ground penetrating; 'very high frequency'. Early radar systems generally operated in VHF as suitable electronics had already been developed for broadcast radio. Today this band is heavily congested and no longer suitable for radar due to interference. |
| P | < 300 MHz | > 1 m | 'P' for 'previous', applied retrospectively to early radar systems; essentially HF + VHF. Often used for remote sensing because of good vegetation penetration. |
| UHF | 300-1000 MHz | 30-100 cm | Very long range (e.g. ballistic missile early warning), ground penetrating, foliage penetrating; 'ultra high frequency'. Efficiently produced and received at very high energy levels, and also reduces the effects of nuclear blackout, making them useful in the missile detection role. |
| L | 1-2 GHz | 15-30 cm | Long range air traffic control and surveillance; 'L' for 'long'. Widely used for long range early warning radars as they combine good reception qualities with reasonable resolution. |
| **S** | 2-4 GHz | 7.5-15 cm | Moderate range surveillance, Terminal air traffic control, long-range weather, marine radar; 'S' for 'sentimetric', its code-name during WWII. Less efficient than L, but offering higher resolution, making them especially suitable for long-range ground controlled interception tasks. |
| C | 4-8 GHz | 3.75-7.5 cm | Satellite transponders; a compromise (hence 'C') between X and S bands; weather; long range tracking |
| **X** | 8-12 GHz | 2.5-3.75 cm | Missile guidance, marine radar, weather, medium-resolution mapping and ground surveillance; in the United States the narrow range 10.525 GHz ±25 MHz is used for airport radar; short-range tracking. Named X band because the frequency was a secret during WW2. Diffraction off raindrops during heavy rain limits the range in the detection role and makes this suitable only for short-range roles or those that deliberately detect rain. |
| Ku | 12-18 GHz | 1.67-2.5 cm | High-resolution, also used for satellite transponders, frequency under K band (hence 'u') |
| K | 18-24 GHz | 1.11-1.67 cm | From German kurz, meaning 'short'. Limited use due to absorption by water vapour at 22 GHz, so Ku and Ka on either side used instead for surveillance. K-band is used for detecting clouds by meteorologists, and by police for detecting speeding motorists. K-band radar guns operate at 24.150 ± 0.100 GHz. |
| Ka | 24-40 GHz | 0.75-1.11 cm | Mapping, short range, airport surveillance; frequency just above K band (hence 'a') Photo radar, used to trigger cameras which take pictures of license plates of cars running red lights, operates at 34.300 ± 0.100 GHz. |
| mm | 40-300 GHz | 1 mm - 7.5 mm | Millimetre band, subdivided as below. Oxygen in the air is an extremely effective attenuator around 60 GHz, as are other molecules at other frequencies, leading to the so-called propagation window at 94 GHz. Even in this window the attenuation is higher than that due to water at 22.2 GHz. This makes these frequencies generally useful only for short-range highly specific radars, like power line avoidance systems for helicopters or use in space where attenuation is not a problem. Multiple letters are assigned to these bands by different groups. These are from Baytron, a now defunct company that made test equipment. |
| V | 40-75 GHz | 4-7.5 mm | Very strongly absorbed by atmospheric oxygen, which resonates at 60 GHz. |
| W | 75-110 GHz | 2.7-4 mm | Used as a visual sensor for experimental autonomous vehicles, high-resolution meteorological observation, and imaging. |

## Cavity Magnetron

A high-powered vacuum tube that generates microwaves using the interaction of a stream of electrons with a magnetic field while moving past a series of open metal cavities (cavity resonators).

## Solid State Transmitter

Solid State Transmitter (SST) is a high power transmitter that uses solid state devices such as MOSFETs, LDMOS, or GaN.

### Solid State Circuit

A circuit that uses solid state components such as transistors, diodes, and integrated circuits (ICs).

## Waveguide

A structure that guides waves, such as electromagnetic waves or sound, with minimal loss of energy by restricting the transmission of energy to one direction.

## Rotating Radar

A radar antenna that rotates at a constant speed.

## Chirp Signal

A signal of frequency increasing (up-chirp) or decreasing (down-chirp) with time.

## Fire Control Radar

A radar that is designed specifically to provide information (mainly target azimuth, elevation, range and range rate) to a fire-control system in order to calculate a firing solution.

## Phased Array Radar

A radar system that uses a large number of antennas to perform beam scanning, a technique that electronically steers a radar beam in a particular direction without physically moving the antenna.

### Phased Array Radar System

A system that uses a phased array antenna to continuously scan the horizon.

### Phased Array Radiation

The radiation pattern of a phased array antenna is the product of the radiation pattern of the individual antennas and the array factor, which depends on the relative phases of the elements.

### Why Phased Array

- No rotating parts
  - No mechanical noise and radiation
  - Easy to maintain
  - Long lifetime
- High gain + Gain control
- Fast update rate
- Coverages of large area
- Flexible and powerful of tracking control
- EMCON (electronic Emission Control) capability
- Multi purpose: surveillance, tracking, fire control, etc.

## Aegis Combat System

An integrated naval weapons system developed by the Missile and Surface Radar Division of RCA, and now produced by Lockheed Martin.

## Track resolution

The ability of a radar to distinguish between two or more targets on the same bearing but at different ranges.

## Radar Detection Range

The maximum distance at which a radar can detect an object.

## Air Surveillance Detection Range

The maximum distance at which a radar can detect an aircraft.

## Air Surveillance Radar

A radar system used to detect and display the presence and position of aircraft.

### Airborne Early Warning Radar

A radar system carried by an aircraft which is designed to detect other aircraft.

## Passive Radar/Direction Finder

A radar system that detects and tracks objects by processing reflections from non-cooperative sources of illumination in the environment, such as commercial broadcast and communications signals.

### Passive Radar

### NMEA-0183

> **NMEA** = National Marine Electronics Association

A combined electrical and data specification for communication between marine electronics such as echo sounder, sonars, anemometer, gyrocompass, autopilot, GPS receivers and many other types of instruments.

| ASCII | Hex | Dec | Use |
| ----- | --- | --- | --- |
| \<CR> | 0x0D | 13 | Carriage Return |
| \<LF> | 0x0A | 10 | Line Feed, end delimiter |
| ! | 0x21 | 33 | Start of encapsulation sentence delimiter |
| $ | 0x24 | 36 | Start of sentence delimiter |
| * | 0x2A | 42 | Checksum delimiter |
| , | 0x2C | 44 | Field delimiter |
| \ | 0x5C | 92 | TAG block delimiter |
| \^ | 0x5E | 94 | Code delimiter for Hex presentation of ISO/IEC 8859-1 (ASCII) characters |
| ~ | 0x7E | 126 | Reserved |

#### NMEA-0183 TTM (Target Tracking Message)

`$--TTM,xx,x.x,x.x,a,x.x,x.x,a,x.x,x.x,a,c--c,a,a,hhmmss.ss,a*hh<CR><LF>`

1. Target Number (00-99)
2. Target Distance
3. Bearing from own ship to target
4. T = True, R = Relative
5. Target Speed
6. Target Course
7. T = True, R = Relative
8. Distance of Closest Point of Approach (CPA)
9. Time to CPA, "-" = Increasing
10. Speed/Distance Units, N = Knots, K = Kilometers, S = Statute Miles
11. Target Name
12. Target Status, A = Active, V = Lost
13. Reference Target, 00-99
14. UTC of data (NMEA 3 and above)
15. Type, A = Automatic, M = Manual, R = Reported (NMEA 3 and above)
16. Checksum

```NMEA-0183 TTM
$RAOSD,180.5,A,179.3,P,2.6,P,178.7,1.3,N*49 $RARSD,-118.1,N,,T,,074051,M*35
$RAOSD,359.3,A,355.2,P,3.3,P,350.5,1.6,N*4F $RARSD,0.00,0.0,5.18,82.1,,,,,,,6,N,N*7B
$RATTM,498,4.29,155.9,T,0.3,74.7,T,1.07,-76.4,N,,T,,074051,M*39
$RATTM,480,5.73,67.0,T,0.2,349.4,T,5.43,35.7,N,,T,,074053,M*17 $RATTM,496,3.60,149.0,T,0.5,28.4,T,1.30,-
68.9,N,,T,,074051,M*33 $RATTM,495,0.87,228.5,T,10.0,322.2,T,0.86,-1.2,N,,T,,074055,M*0C
$RATLB,481,,470,,469,,468,,467,,441,,210,,399,,383,,381,,380,,132,,345,,344,*4A
$RATTM,492,0.75,281.7,T,1.2,352.7,T,0.72,5.6,N,,T,,074054,M*10
$RATTM,489,4.44,330.6,T,3.0,357.6,T,0.30,795.4,N,,T,,074054,M*18
$RATTM,481,5.17,39.6,T,0.2,328.2,T,3.49,73.5,N,,T,,074055,M*12
$RATTM,470,4.32,334.1,T,2.8,357.7,T,0.63,472.5,N,,T,,074054,M*19
$RATTM,469,2.46,283.5,T,1.6,179.3,T,2.35,8.8,N,,T,,074054,M*1F
$RATLB,339,,66,,499,,273,,497,,500,,498,,480,,496,,495,,492,,489,,481,,470,*73
$RATTM,468,2.20,285.4,T,1.3,172.1,T,2.05,10.3,N,,T,,074054,M*24
$RATTM,467,2.26,284.3,T,5.1,128.7,T,1.52,12.9,N,,T,,074054,M*2D $RAOSD,359.3,A,355.2,P,3.3,P,351.6,1.8,N*43
$RARSD,0.00,0.0,5.18,82.1,,,,,,,6,N,N*7B $RATTM,441,0.86,183.5,T,4.2,31.6,T,0.85,3.4,N,,T,,074054,M*2F
$RATTM,210,4.69,156.2,T,0.4,79.3,T,0.94,-83.9,N,,T,,074053,M*33
$RATTM,399,1.30,196.8,T,3.9,342.8,T,1.29,12.1,N,,T,,074054,M*2F $RATTM,383,4.39,229.2,T,2.5,2.9,T,4.28,-
67.1,N,,T,,074054,M*05 $RATLB,469,,468,,467,,441,,210,,399,,383,,381,,380,,132,,345,,344,,339,,66,*7D
$RATTM,381,6.68,142.8,T,0.6,65.0,T,2.36,-119.8,N,,T,,074055,M*05 $RATTM,380,6.48,147.0,T,4.5,237.7,T,5.85,-
25.2,N,,T,,074055,M*05 $RATTM,132,2.06,189.3,T,0.6,105.6,T,0.82,-31.8,N,,T,,074056,M*0B
$RATTM,345,2.89,141.7,T,1.4,1.7,T,1.36,-79.0,N,,T,,074057,M*02 $RATTM,344,2.89,141.8,T,1.4,1.4,T,1.37,-
78.5,N,,T,,074057,M*0A $RATTM,339,2.92,172.5,T,1.1,101.1,T,0.69,-45.4,N,,T,,074056,M*02
$RATTM,66,5.58,196.0,T,7.3,175.1,T,2.00,-29.4,N,,T,,074056,M*35
```

#### NMEA Checksum

- Start with a `*` and consists of 2 characters representing a hexadecimal number. The checksum is the 8-bit exclusive OR (XOR) of all characters between, but not including, the `$` and `*`.

#### NMEA Checksum Code Example

```python
cdef bytes __HEX_MAP__ = b'0123456789ABCDEF'
cdef u8 __HEX_RMAP__[256]

for i in range(16):
    __HEX_RMAP__[(<u8> __HEX_MAP_BUFFER__[i])] = i
    __HEX_RMAP__[(<u8> __HEX_LOWER_MAP_BUFFER__[i])] = i

cdef bint checksum(bytes raw):
    cdef u8 checked = 0
    cdef char *buffer = <char *> raw
    cdef u32 length = len(raw)
    for i in range(1, length-3):
        checked = checked ^ buffer[i]
    cdef u8 inSentence =
        (__HEX_RMAP__[(<u8> buffer[length-2])] << 4) +
        __HEX_RMAP__[(<u8> buffer[length-1])]
    return isSentence == checked

cdef int calculateSum(bytes sentence):
    cdef u8 checked = 0
    cdef char i
    for i in sentence:
        checked = checked ^ i
    return checked & 255
```

### ASTERIX

ASTERIX (All Purpose Structured Eurocontrol Surveillance Information Exchange) is a standard for the exchange of air traffic services (ATS) information. It is developed and maintained by the European ATS organization Eurocontrol. ASTERIX is surveillance data format which is being adopted by the world users community as the universal standard in this domain today.

`<CAT = 048><LEN><FSPEC><Items of the first record><...><FSPEC><Items of the last record>`

- CAT: Category is a 1-byte field that indicates the category of the record.
- FSPEC: Field Specification is a 1-byte field that indicates the presence or absence of each data item in the record.
- Items: Data items are the actual data that is transmitted in the record.
- LEN: Length is a 2-byte field that indicates the total length of the record in bytes.

#### ASTERIX 048 (Monoradar Target Reports)

#### ASTERIX 048 Item 030 (Measured Position in Polar Coordinates)

---

# Radar Connectivity

## RS232 Serial Port

A standard for serial communication transmission of data.

- DRS: Data Rate Selector
- CTS: Clear To Send
- RTS: Request To Send
- RI: Ring Indicator
- CD: Carrier Detect
- TXD: Transmit Data
- RXD: Receive Data
- DTR: Data Terminal Ready
- GND: Signal Ground

- RS232 Direct Cable:
- RS232 Cross Cable:
- Serial to USB cable
- Windows COM Port
  - COM: Communication Port

### Example Code

```python
import serial

ser = serial.Serial(
    port='/dev/ttyUSB0',
    baudrate=9600,
    parity=serial.PARITY_ODD,
    stopbits=serial.STOPBITS_TWO,
    bytesize=serial.SEVENBITS
)

print(ser.name)
ser.write(b'hello')
ser.close()
```

### Serial Expander

A device that allows a serial port to be connected to a computer using a USB port.

- RS232 splitter (port replicator)

### Data Distributor

- C-MAN: Coastal-Marine Automated Network

---

# Basic Communication

## Signal Modulation

The process of varying one or more properties of a periodic waveform, called the carrier signal, with a modulating signal that typically contains information to be transmitted.

### Pulse Code Modulator

A device that samples an analog signal and converts it into a series of digital pulses.

- TX section
  - Analog message signal (voice, music, video)
  - LPF: Low Pass Filter (cut off frequency)
  - Sampler: Sample the analog signal at a fixed rate
  - Quantizer: Quantize the sampled signal into a discrete set of levels
  - Encoder: Encode the quantized signal into a binary code
- PCM output (pulse code modulated signal)
- CHANNEL (transmission medium)
  - Regenerative repeater: Reconstruct the PCM signal
- RX section
  - Regeneration circuit: Reconstruct the PCM signal
  - Decoder: Decode the binary code into a quantized signal
  - Reconstruction filter: Reconstruct the analog signal
  - Destination: Analog message signal (voice, music, video)

## Fourier Transform

A mathematical transform that decomposes a function (often a function of time, or a signal) into its constituent frequencies.

## Convolutions

A mathematical operation on two functions that produces a third function expressing how the shape of one is modified by the other.

## Quantization

The process of mapping input values from a large set (often a continuous set) to output values in a (countable) smaller set.

## Sampling and Spectrum

### Sampling

The process of converting a continuous analog signal to a discrete digital signal.

### Spectrum

The frequency domain representation of a signal.

### Nyquist Frequency

The minimum rate at which a signal can be sampled without introducing errors.

## LPF (Low Pass Filter)

A filter that passes signals with a frequency lower than a selected cutoff frequency and attenuates signals with frequencies higher than the cutoff frequency.

## IQ-Modulator : Complex Signal

A modulator that modulates a carrier signal with a complex signal.

## Modulation Format

The way in which information (message signal) is conveyed over a signal (carrier signal).

- BPSK: Binary Phase Shift Keying
  - 2-level symbol -> 1 bit/symbol
- QPSK: Quadrature Phase Shift Keying
  - 4-level symbol -> 2 bit/symbol
- 8QAM: 8-Quadrature Amplitude Modulation
  - 8-level symbol -> 3 bit/symbol
- 16QAM: 16-Quadrature Amplitude Modulation
  - 16-level symbol -> 4 bit/symbol

## Channel Coding

A process where redundant data is added to a digital message to be transmitted over a noisy channel.

### RS decoding (Reed-Solomon)

A block code that adds redundancy to a message by using a non-binary finite field.

> GPT

RS Decoding, or Reed-Solomon decoding, is commonly utilized in data transmission and storage systems to detect and correct errors. Here's a general procedure:

1. **Input**: RS decoding begins with receiving the code symbols. This incorporates both actual data as well as the redundant symbols added by RS encoding.
2. **Syndrome Calculation**: The decoder computes what is known as the "syndrome" values. The count of syndromes is equivalent to the quantity of redundant symbols appended during the encoding process.
3. **Identification of Errors or Erasure**: If all syndrome values are zero, there's no error. However, if there's any non-zero syndrome, the system realizes there are errors or erasures to counteract.
4. **Berlekamp–Massey Algorithm**: To find out the error location polynomial, this iterative algorithm is employed.
5. **Chien Search**: It is used to find the roots of the error location polynomial. The roots of this polynomial represent the error locations.
6. **Forney Algorithm**: This algorithm calculates error values using the error location and error evaluator polynomials.
7. **Correction**: At this stage, the original message is corrected using the determined error location numbers and error values.
8. **Output**: The corrected output of RS decoder is then sent for further processing or use.
This is a general procedure and may slightly vary based on the type of RS decoder or real-world conditions. Remember, the goal is to correct errors that occurred during data transmission/storage and to retrieve the original, unaltered data as closely as possible.

## Multiple Access

The ability of a communications system to support multiple users simultaneously.

- FDMA: Frequency Division Multiple Access
- TDMA: Time Division Multiple Access
- CDMA: Code Division Multiple Access

### Code Division Multiple Access

---

# Automatic Dependent Surveillance–Broadcast (ADS-B)

Automatic Dependent Surveillance–Broadcast (ADS-B) is an aviation surveillance technology and form of Electronic Conspicuity in which an aircraft (or other airborne vehicles such as drones approved to fit "ADS-B Out") determines its position via satellite navigation or other sensors and periodically broadcasts its position and other related data, enabling it to be tracked.

## ADS-B Connection

- GNSS: Global Navigation Satellite System
- COMM: Communication
- ATC: Air Traffic Control
- ARTCC: Air Route Traffic Control Center
- TIS-B: Traffic Information Service-Broadcast

## ADS-B Application

- Aircraft will broadcast own information.
- ATC will recieve the information.
- It can be used as P2P communication.
- Key part of ICAO's approved aviation surveillance technology.
  - ICAO: International Civil Aviation Organization
- Aircraft operators are encouraged to equip their aircraft with ADS-B Out.
- ATC can provide better and more fuel-efficient routing.

## Operating Frequencies

- 1090 MHz: Common usage
- 978 MHz: Mode S Transponder (S for Surveillance)

## ADS-B Data Format (Binary based)

### B-Frames: Binary Frames: 112 bits

| Bit | #bits | Abbreviation | Information |
| --- | ----- | ------------ | ----------- |
| 1-5 | 5 | DF | Downlink Format |
| 6-8 | 3 | CA | Transponder Capability |
| 9-32 | 24 | ICAO | ICAO 24-bit Aircraft Address |
| 33-88 | 56 | ME | Message, Extended Squitter |
| (33-37) | (5) | (TC) | (Type Code) |
| 89-112 | 24 | PI | Parity / Interrogator Identifier |

### Airborne position: 46bits

| Field | | MSG | ME | BITS |
| ----- | - | --- | -- | ---- |
| Type Code | TC | 33-37 | 1-5 | 5 |
| 9-18: with barometric altitude | | | | |
| 20–22: with GNSS altitude|||||
| Surveillance Status |SS| 38-39 | 6-7 | 2 |
| 0: No condition information | | | | |
| 1: Permanent Alert (Emergency) | | | | |
| 2: Temporary Alert (Ident) | | | | |
| 3: SPI (special position identification) | | | | |
| Single Antenna Flag | SAF | 40 | 8 | 1 |
| Encoded Latitude | LAT | 41-52 | 9-20 | 12 |
| Time | T | 53 | 21 | 1 |
| CPR (Compact Position Reporting) Format | CPRF | 54 | 22 | 1 |
| 0: even frame | | | | |
| 1: odd frame | | | | |
| Encoded Latitude | LAT-CPR | 55-71 | 23-39 | 17 |
| Encoded Longitude | LON-CPR | 72-88 | 40-56 | 17 |

> The CPR positioning system is a specialized positioning system and cannot be directly used. The message must be decoded and transformed into the regular position.

## ADS-B in Military Use

- Identification of commercial aircraft
- Replacement of IFF (Identification Friend or Foe) system
- Improvement of situational picture
- Military ATC (Air Traffic Control)
- Low cost solution for military aircraft data

### Challenge of ADS-B in Military Use

- Update rate: Much faster than AIS (Automatic Identification System)
- Correlation with air surveillance radar
- Data volume
- UI design must be very specific and simple to optimize response time
- Real-time data processing

---

# Automatic Identification System (AIS)

An automatic tracking system that uses transceivers on ships
and is used by vessel trafﬁc services (VTS).

- When satellites are used to receive AIS signatures, the term
Satellite-AIS (S-AIS) is used.
- AIS information supplements marine radar, which continues to be the primary method of collision avoidance for water transport.

## AIS Connections & Variants

### Type

- vessel based: The 2002 IMO SOLAS Agreement included a mandate that required most vessels over 300GT on international voyages to ﬁt a Class A type AIS transceiver.
- Terrestrial Based : Shipboard and land-based AIS transceivers have a horizontal range that is highly variable, but typically only up to about 74 kilometres (46 mi). Approximate line-of-sight propagation limitations mean that terrestrial AIS (T-AIS) is lost beyond coastal waters.
- Satellite AIS : *Challenge* : very large numbers of AIS messages simultaneously -> TDMA. Various frequencies and orbit height will be used.

> TDMS: Time Division Multiple Access

### AIS Class A

- Self-organizing time-division multiple access (SOTDMA)
- Targeted at large commercial vessels
- Class A units must have
  - an integrated display
  - tx power of 12.5 W
  - interface capability with multiple ship systems
  - sophisticated selection of features and functions

### AIS Class B

- Carrier-sense time-division multiple access (CSTDMA) or SOTDMA
- Aimed at lighter commercial and leisure markets

### Other AIS Classes

- Base stations: SOLAS for receiving AIS signals from vessels
- Aids to navigation (AtoN): Shore- or buoy-based transeiver with Fixed-access time-division multiple access (FATDMA) designed to collect  and transmit data related to sea and weather conditions as well as relay AIS messages to extend network coverage
- Search and recue transceiver (SART): emergency distress beacon which operates using pre-announced time-divided multiple-access (PARDMA).

### AIS frequencies (vessel & terrestrial based)

- AIS uses the globally allocated Marine Band channels 87 and 88.
- AIS uses the high side of the duplex from two VHF radio "channels" (87B) and (88B)
  - Channel A 161.975 MHz (87B)
  - Channel B 162.025 MHz (88B)

Most AIS transmissions are composed of bursts of several messages. In these cases, between messages, the AIS transmitter must change channel.

### AIS Regulation 1

- International Regulation : IMO
  - IMO : International Maritime Organization
  - Vessel bigger than 300 gross-ton must install AIS.
  - For the coastal sailing, AIS must be turned on.
  - Main purpose : Collision avoidance.
  - Other purposes : Position tracking, behavior monitoring, etc.
  - Due to international : Soft enforcement.

### AIS Regulation 2

- Thai Law : Marine Department (Ministry of Transportation)
  - Vessel bigger than 300 gross-ton must install AIS.
  - Vessel with more than 12 passengers
  - Vessel at sea, AIS must be turned on all the time.
  - Law violation : Purge of Certiﬁcation
  - How is the law enforced?
  - Main purpose : Safety, Search and Rescue, and Collision avoidance.

### AIS Regulation 3

- Thai Law : Fishery Department (Ministry of Agriculture)
  - Small ﬁshing boat 5-30 gross-ton must install AIS.
  - Bigger ﬁshing boat bigger than 30 gross-ton : VMS
  - Very confusing of enforcement
  - How is the law enforced?
  - Main purpose : Fishery regulation.

### AIS data example

```txt
!AIVDO,1,1,,,18SnoL0P?w>tSF0l4Q@>4?wv1P00,0*2B !AIVDM,1,1,,B,4h5J8gAvB:4K9W=lnr7?NLg02>4E,0*68
```

### AIS Base64 data

### AIS Data Format

> long table

### AIS: More Position & Application

### Why More AIS?

- Identiﬁcation of vessel + additional data
- High volume of data
- Satellite AIS : Global positioning available
- Relative cost effective
- Acceptable update rate

### Drawback of AIS

- Data can be faked
- Vessel can turn of the equipment
- Un reliable timestamp

For system with high creditability, AIS cannot be single source of truth. AIS should be used together with other type of sensor e.g. radar.

### AIS: Behavior Analysis

### Route Extraction

- Extract route from AIS data
- Route is a sequence of waypoints
- Waypoint is a position with time stamp

---

# Satellite Communication

## Geostationary Orbit (GEO)

- From west to east following Earth’s rotation : taking 23 hours 56 minutes and 4 seconds – by travelling (exactly the same rate as Earth).
- This makes satellites in GEO appear to be ‘stationary’ over a fixed position.
- In order to perfectly match Earth’s rotation, the speed of GEO satellites should be about 3 km per
second at an altitude of 35,786 km.
- Mostly used for telecommunication.

## Low Earth Orbit (LEO)

- It is normally at an altitude of less than 1000 km but could be as low as 160 km above Earth.
- LEO satellites do not always have to follow a particular path around Earth in the same way.
- It is the orbit most commonly used for satellite imaging.
- It is also the orbit used for the International Space Station (ISS)

## Medium Earth orbit (MEO)

- MEO comprises a wide range of orbits anywhere between LEO and GEO.
- It is similar to LEO in that it also does not need to take specific paths around Earth, and it is used by a variety of satellites with many different applications.
- It is very commonly used by navigation satellites e.g. Galileo system.

## Sun-Synchronous Orbit (SSO)

- SSO pass the North and South Pole precisely.
- Even a deviation within 20 to 30 degrees is still classed as a polar orbit.
- Polar orbits are a type of low Earth orbit, as they are at low altitudes between 200 to 1000 km.
- It always observes a point on the Earth as if constantly at the same time of the day.
- Application : Photo at the same time of the day for difference observation

## Geostationary Transfer Orbit (GTO)

- Special deployment of GEO Satellite with simplification method of launching

## Satellite Orbit Comparison

## Thuraya Satellite Phone

- Thuraya is a regional satellite phone provider.
- Thuraya satellite phone is a dual mode phone that can operate in both satellite and GSM mode.
- Thuraya satellite phone can be used in Thailand.

### Thuraya Satellite Communication

## ThaiComm

### ThaiComm Coverage Area

## Starlink

- Small LEO Satellite
- 5,000 Satellites are deployed.
- 12,000 Satellites are planned to deploy.
- 42,000 Satellites will be expanded to deploy.

## Satellite Traffic

## Satellite Communication Advantages

- BLOS communication (Beyond Line of Sight)
- Coverage area
- Obstacle independent
- Relative simple deployment (Band dependent)

## Satellite Communication Disadvantages

- Cost
- Security
- Coverage area
- Complicated deployment (Band dependent)

> Recommendation in Military Use : Admin Only, No Operational

---

# Sonar

Sonar (sound navigation and ranging or sonic navigation and ranging) is a technique that uses sound propagation to navigate, measure distances (ranging), communicate with or detect objects on or under the surface of the water, such as other vessels.

## Submarine Sonar Dome

## Electromagnetic Wave in Water

## Active Sonar Principle

## Sound Speed in Water

## Analogy : Light Refraction

## Sonar Shadow Zone

## Sonar Screen Example

## Anti-Submarine Warfare

## Towed Sonar

## Sonobuoy

## Sonar in Military Use

- Very unreliable : No specific position and classification.
- Sonar datum will be explicitly plotted.
- Data from sonar will not treated as track.
- Data from sonar will not distributed.
- Sonar datum must be analyzed by a trained personnel.
- Lack of sonar quality : Submarine is fearsome.

## Side Scan Sonar : Survey

## Side Scan Sonar

> GPT

- **Sonar**: Sonar, an acronym for sound navigation and ranging, is a technique that utilizes sound propagation (usually underwater) to navigate, communicate, detect, or measure distances.
- **Submarine Sonar Dome**: This is the housing structure on a submarine that holds the sonar equipment, which protects it from physical damage and allows it to operate efficiently.
- **Electromagnetic Wave in Water**: This refers to how electromagnetic waves, including light and radio waves, behave when they propagate through water. Unlike in air, electromagnetic waves can be quickly attenuated in water.
- **Active Sonar Principle**: Active sonar works by emitting a sound pulse and then listening for the echo of that pulse. It's mainly used to detect and determine the position and distance of underwater objects.
- **Sound Speed in Water**: The speed at which sound travels underwater is roughly 1,480 meters/second - much faster than in air. This speed can be affected by factors like temperature, salinity and pressure.
- **Analogy: Light Refraction**: Just like light bends (refracts) when it passes from one medium (e.g., air) to another (e.g., glass or water), sound waves can also refract when they travel through layers of water with different temperatures or salinities.
- **Sonar Shadow Zone**: This is an area that can't be scanned by sonar due to limitations in the sonar technology or environmental conditions. It might be too far, too close, or at an awkward angle for the sonar to detect.
- **Sonar Screen Example**: A sonar screen shows the results of sonar scans, typically displaying objects and their relative positions and distances.
- **Anti-Submarine Warfare**: A military strategy used to detect and destroy enemy submarines, often involves the use of sonar.
- **Towed Sonar**: This is a type of sonar system where the sonar device is physically towed behind a vessel, allowing for a larger scan area and better detection capabilities.
- **Sonobuoy**: A small, floatable sonar system that is dropped or ejected from an aircraft or ship for underwater surveillance or scientific data collection.
- **Sonar in Military Use**: It's used for detection and communication. However, its reliability can be variable, and it may require trained personnel for data analysis. The quality of sonar data is crucial in military strategy, especially when dealing with submarines.
- **Side Scan Sonar: Survey**: Side-scan sonar is used to create images of large areas of the seafloor. It's often used in surveys of underwater geological formations or for searching for sunken objects.
- **Side Scan Sonar**: This type of sonar sends out sound waves in a fan-shaped beam to either side of a towed sensor (towfish). It is used to produce detailed images of the sea bottom structure and potential objects on it.

---

# Data Processing Architecture

## The Stone Age : Local Storage

- Data will be stored in local computer
- Extremely easy to deploy
- No network
- No concurrent user
- Limitation of data volume
- User interface : CLI (Terminal)
- Some application proves itself as a very robust application.

## GUI with Database

- Data will be stored in database server
- OS specific
- Concurrent user is possible.
- Complicated GUI and DB deployment
- Limitation of data volume and concurrent use
- Ease of use? (Intuitive)

## Visual Basic 6

- Good example for ease of development, bad example for software design.

## LAMP Stack (Linux, Apache, MySQL, PHP)

- Grandfather of All Webs
- Extremely robust
- Ease of deployment (Server & Client Side)
- Relative good concurrent processing
- Software design trends to be messed up.
- Hard to scale

## Common Object Request Broker Architecture

- CORBA is a standard defined by the Object Management Group (OMG) designed to facilitate the communication of systems that are deployed on diverse platforms.
- CORBA enables collaboration between systems on different operating systems, programming languages, and computing hardware.
- CORBA uses an object-oriented model although the systems that use the CORBA do not have to be object-oriented.
- CORBA is an example of the distributed object paradigm.

## SOAP Web Service

- SOAP is a messaging protocol specification for exchanging structured information in the implementation of web services in computer networks.
- Its purpose is to provide extensibility, neutrality, verbosity and independence.
- Stand for **Simple Object Access Protocol**

## RESTFull Web Service

- REST is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other.

## Web Service

- Web-Service can be seen as Remote Procedure Call (RPC).
- Ease of use and deployment
- Real time data consumption
- Simple but robust approach
- The methods are more and more simplified.

## Monolithic vs. Microservice

### Advantage of Microservice

- Agile development process
- Flexible scaling
- Continuous deployment
- Highly maintainable and testable (?)
- Independently deployable
- Technology flexibility
- High reliability (?)

### Disadvantage of Microservice

- Development sprawl
- Exponential infrastructure costs
- Added organizational overhead
- Debugging challenges
- Lack of standardization
- Technology flexibility
- Lack of clear ownership

## Databus Architecture

- Flexible data exchange between services
- In some case : Increase network load
- In some case : Decrease network load
- Robust against system fail
- Single point of failure!!!
- Example : Kafka, RTI, ZeroMQ, RabbitMQ, Redis

## CAP Theorem

- Consistency
- Availability
- Partition Tolerance

## Database Replication

- Each node : Same Data
- Semi distributed data storage and process
- Single point of failure
- Automated backup
- Limitation of scale
- Additional procedure for data recovery
- ACID compliance
- Relative High Throughput, Consistency Warranty but No Error Tolerance

## Consistent Hashing

- Distributed data storage and process
- Each node : Different Data
- Automated backup
- No data recovery needed
- Eventually Consistency
- Highly scalable
- High Throughput, Error Tolerance but No Consistency Warranty

## Map Reduce

- Distributed data process
- Inspired by Functional Programming -> Google Big Table
- Beware : Brute-Force method
- It can be very complicated.

## ETL (Extract, Transform, Load)

- Data **Warehouse**: A data warehouse is a central repository of information that can be analyzed to make better-informed decisions.
- Data **Lake**: A data lake is a centralized repository that allows you to store all your structured and unstructured data at any scale.
- Data **Mart**: A data mart is a subset of a data warehouse that is designed for a particular business line, such as finance, marketing or sales.

---