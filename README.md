# Open Source Coordinate Measuremnt Arm

This opensource coordinate measurement arm registers the x-, y- and z-coordinate of the pointer by reading the 5 angles of the joints. 

## Project Description

Compared to conventional proprietary CMMs, this one can be extended to fit specific requirements, because it open source as possible. No commercial CAD tools are needed. The construction kit approche allows changes without expensive tools like 3d printers. Most parts are parameterized.



## Current Status 

- active maintained


## Dependencies

- are referenced as submodules:
    - `xyzcad` implicit surface geometry based CAD software to create the 3d printed parts
    - `Fuzzyometry` implicit chamfer library for `xyzcad`
    - `SpiroBrixx` building blocks for instant mechanical prototyping
    - `cmm-host-software` runs on the host PC to record raw data from the CMM, minimal GUI tool, no visualization
    - `read-rotary-encoder` Arduino software to get data for the `cmm-host-software`
    - `rotary-encoder-protection` electronic in each plug of the rotary encoders to protect the against electrical damage
    - `OSH-CMM-LogicBoard` main electronic board carrying the Arduino, reads the angles of the 5 rotary encoders
    - `CCM-Arm` extended/modified incomplete OSH CMM arm project with visualizing host software and kinematic coordinate calculation

## License

- Software: "AGPL-3.0-or-later"
- Hardware: "CERN-OHL-S-2.0"
