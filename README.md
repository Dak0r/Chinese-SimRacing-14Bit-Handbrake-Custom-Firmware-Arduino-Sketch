# Chinese-SimRacing-14Bit-Handbrake-Custom-Firmware (Arduino Sketch)
Alternative Firmaware for Chinese "14 Bit" Sim Racing Handbrake by Daniel Korgel

The 12 and 14 Bit Version of the chineses SimRacing Handbrake use an Arduino Pro Micro and a hall sensor.

This sketch is desigend as a replacement firmware to allow modifcations like connecting more buttons to the arduino and so using more of it's potential. 


# How to use

### 1. Install the Arduino Joystick Library from by Matthew Heironimus:

* Repository: https://github.com/MHeironimus/ArduinoJoystickLibrary
* Director Download: https://github.com/MHeironimus/ArduinoJoystickLibrary/archive/master.zip

If your IDE is using default directories, you can execute the deploy.at to Install the library, otherwise you need to copy the Joystick directory into your Arduino/libraries directory manually.

### 2. Download and Deploy to Handbrake Arduino

Download this repository, open the "ChineseHandbrakeCustomFirmware.ino" with your Arduino IDE.
Conntect your Handbrake and select the corresponding COM port of the device, which will be titled "Arduino Leonardo".
Select "Arduino Leonardo" as the Board Type.
Compile and Deploy the Sketch.

Done! 


# About

Within the handbrake there's a simple PCB with an Arduino Pro Micro and a Hall Sensor.
On Version 3.0 of the Handbrake PCB the hall sensor is conntector to GND, VCC and A2. The PCB some anotherlead to pin 10, but it's not connected. 
Pin 3 and pin 1 were also connected on my board, but there are no leads going anywhere, so I assume they are just for stabilization.


**Note: I know that there's at least a version 4.0 of this PCB, but I don't know the exact differences.
