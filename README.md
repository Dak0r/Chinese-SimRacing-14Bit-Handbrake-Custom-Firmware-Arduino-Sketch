# Chinese-SimRacing-14Bit-Handbrake-Custom-Firmware (Arduino Sketch)
Alternative Firmaware for Chinese "14 Bit" Sim Racing Handbrake by Daniel Korgel

<img src="https://i.imgur.com/D5v82bh.jpg" width="350" alt="Product image of the handbrake">

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

On the pcb titled *version 3.0* the hall sensor is conntector to GND, VCC and A2. The PCB some has another lead to pin 10, but it's not connected to anything else, due to a missing resistor.
Pin 3 and pin 1 of the arduino were also soldered on my board, but there are no leads going anywhere. To be sure I measured both and found that they are not connected to anything that's measurable on the pcb. I assume they are just soldered for stabilization.

<img src="14bit%20v3%20images/pcb_v3_top_anot.jpg?raw=true" width="350" alt="Top View of the v3 PCB"/>

[Top View of the v3 PCB](14bit%20v3%20images/pcb_v3_top_anot.jpg?raw=true "Top View of the v3 PCB")

<img src="14bit%20v3%20images/pcb_v3_bottom_anot.jpg?raw=true" width="350" alt="Bottom View of the v3 PCB"/>

[Bottom View of the v3 PCB](14bit%20v3%20images/pcb_v3_bottom_anot.jpg?raw=true "Bottom View of the v3 PCB")

**Note: I know that there's at least a version 4.0 of this PCB, but I don't know the exact differences.**
