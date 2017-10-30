# Control of a XYTable
 Author: Janine Müller

## Description
A XY-Table is a construction built from two linear tracks, which are mounted perpendicular. To allow a movement in two directoins (x and y) the second track is mounted on the carriage of the first track. The x axis has a traveling distance of 2500mm and the y axis of 200mm.  
Both axis are driven by TRINAMIC motors and connected to the PC via RS232.  
This software allows to do measurements with this XYTable on scintillating fibres and fibre mats from scintillating fibres. For this a current source operated via RS232 allows to pilot UV-LEDs to excite the fibre(s).  
To get the response of the scintillating fibre (or mat) a spectrometer is read out via USB.  
It is possible to do measurements in x and y direction as well as only in x direction e.g. to determine attenuation lengths.  
Special mounting setups for the spectrometer allow as well a angular dependent measurement of the fibre response.

The repository contains the source code as well as CMakeLists and a GUI version to operate such system.

## Requirements to run terminal program

Availability of the following libraries (author: Janine Müller):
* [LEDClass][1]
* [SpectrometerClass][2]
* [MotorControl][3]
* [RS232Communication][4]


## Requirements  to run GUI
- QT5 (in .bashrc: export CMAKE_PREFIX_PATH=/usr/local/Qt-5.8.0/)
- QT5 uses different number format (n .bashrc: export LC_NUMERIC=en_US.UTF-8)

## How to run the control





[1]: https://git.e5.physik.tu-dortmund.de/jmueller/LEDClass
[2]: https://git.e5.physik.tu-dortmund.de/jmueller/SpectrometerClass
[3]: https://git.e5.physik.tu-dortmund.de/jmueller/MotorControl
[4]: https://git.e5.physik.tu-dortmund.de/jmueller/RS232communication