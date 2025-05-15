
# User Manual OSH-CMM

The measurement arm can only be used as peripheral USB device in combination with a host computer. It is powered by the computer, which also stores the measured values. 

## Requirements

Minimum system requirements:
* PC or Mac
* OS: _Microsoft Windows 11_, _Ubuntu Linux 24.04 LTS_ or _Mac OS X 15_
* 2 CPU cores with 1 GHz
* 1 GB free HDD space
* 8 GB RAM
* 1 USB 2.0 host port
* single 1280 x 720 screen
* keyboard

## Setup

The host software bundled with all _java_ and other third party components can be downloaded as a single `.zip` file:

https://github.com/TheTesla/CCM-Arm/releases/download/v0.9/CMM-5-DOF-Host-Software-windows-amd64.zip

After extracting the archive, the `CMM_DXF_V8.exe` must be started to run the software. This is a portable app, no installation is required. After starting the software, an interactive window will appear. This is the user interface, which visualizes the measured points.

![GUI without device](host_software_0.png)

The host software can be demonstrated without the measurement arm by using the mouse.

Make sure, the pointer of the measurement arm is in the reference position. This is needed to get the best precision. While the arm is in this position, connect the measurement arm to the host computer. Now, an extra serial port should be listed, e. g. `COM6`:

![GUI with device connected](host_software_1.png)

The host software checks all available serial ports, until it finds the measurement arm. When the arm is found, there should be a line drawing of the measurement arm visible in the interactive window, which moves, if the arm is moved:

![GUI with connection established](host_software_2.png)

Now, mouse input is disabled and only the arm data is processed.

## Measure coordinates

Use the pointer of the arm, point it to the position, which should be recorded. Press `.` on the keyboard to record the point and mark it with a dot. To draw lines, start the line with `1` and add corners with `0`. Press `5` to mark a hole.

The recorded data can be stored by clicking `PtCld`. This exports a point cloud file.

## End work

After all the emasurement work is done. The USB cable should be unplugged and the program can be closed by clicking `Quit`. The pointer of the arm should be placed in the reference position to reduce mechanical forces.

