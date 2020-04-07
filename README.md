
![](https://raw.githubusercontent.com/roverwing/RoverWingHardware/master/docs/images/roverwinglogo-pathconverted.png)

Introduction
============
RoverWing is an extension board  (or "wing", following Adafruit's terminology) for Adafruit's [Feather boards](https://www.adafruit.com/feather).
This board  provides motor drivers, Inertial Motion Unit (IMU), and connection ports for servos, sonars, GPS,
and other peripherals commonly used by mobile robots. It also contains a microcontroller preloaded with firmware
to control these peripherals, which communicates with the Feather board using I2C protocol, thus freeing resources
of the Feather board for other purposes.

The RoverWing was heavily influenced by Adafruit's [CRICKIT](https://www.adafruit.com/crickit) board
(in particular, it has exact same dimensions and  mounting holes as the CRICKIT board). However, unlike CRICKIT,
it is intended for use with more powerful 6-12V motors and provides a slightly different set of peripherals.

Below is the list of key features of the RoverWing:

* Can be powered by 7-14V power source; contains a voltage regulator providing power to the Feather board

* Only uses 2 pins (SDA and SCL) of the Feather board.

* Contains on-board microcontroller, which takes care of low-level operations such as counting motor encoder pulses, using preloaded firmware

* Contains on-board 6DOF  Inertial Motion Unit (IMU),  based on ICM-42605 chip
  by Invensense, which can be used for tracking robot orientation in space

* Provides the hardware and firmware support for connecting the following external peripherals

  - Motors: two brushed DC motors, at up to 2.9A at 14V per motor
  - Quadrature encoders for each motor
  - Sonars: support for three HC-SR04 or compatible ultrasonic sensors (sonars)
  - Servos: four servos (5V)
  - Six analog inputs (3.3V)
  - NeoPixel smart LED (see note on power limit below)
  - GPS  sensor
  - one  additional I2C device

The RoverWing uses same connectors for power supply, motors, encoders, and I2C
sensors as the [REV Robotics Expansion hub](http://www.revrobotics.com/rev-31-1153)  used in [First Tech Challenge](https://www.firstinspires.org/robotics/ftc)  robotics competition, so it can
be easily used with the same motors and sensors.

![alt text](https://raw.githubusercontent.com/roverwing/RoverWingHardware/master/docs/images/MainView.jpg)
   RoverWing (without the Feather), top view.

For complete documentation of RoverWing board, please visit https://roverwing-board.readthedocs.io/.

To use RoverWing board, you need to install [RoverWing library for Arduino](https://github.com/roverwing/RoverWingLibrary).
