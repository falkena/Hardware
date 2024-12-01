# Hardware
Some hardware extensions i developed for RaspberryPi.

Boards are made for rail - din enclosures.

Boards and schematics are published under Open Hardware License:
http://www.ohwr.org/licenses/cern-ohl/v1.2

DigitalIO
----------
MCP23017 based board supporting 8 digital inputs/outputs.
Inputs are opto-isolated and can be used up to 24V DC.
Outputs are relay driven. More details can be found in
documentation for used components.

Board can be driven for example with Pi4J.

AnalogI
-------
MCP3424 based board supporting 4 analog inputs.
Inputs are opto-isolated and can measure signals up to 10V DC.

Board can be driven for example with Pi4J.


Very special thanks to the guys from http://www.mikrocontroller.net

Automation board
----------------

![Top view](./MainBoard/MainBoardTop.svg)
![Bottom view](./MainBoard/MainBoardBottom.svg)

Automation board for Raspberry PI. Designed to work with input voltage 15-24V.
Provides I2C connector, two wireless receiver for 433 and 868 MHZ as well PWM
fan 4 pin. Additional 2 pin connector can be used for shutdown with help of
`gpio-shutdown` overlay. Required 5V supply is done via MP1584 and MP2482 based
dc/dc step-down modules. See `modules` Eagle library for details.

Rain sensor
-----------

![Top view](./Regensensor/RainSensorTop.svg)
![Bottom view](./Regensensor/RainSensorBottom.svg)

LM358 OpAmp based rain sensor detector. Designed to work with input voltage 15-24V.
Provides input and 10V digital outputs as well possibility to control heating.

![Top view](./Regensensor/KammSensorTop.svg)
![Bottom view](./Regensensor/KammSensorBottom.svg)

Drop sensor is based on https://github.com/ranseyer/home-automatics/tree/master/Rain-Sensor/Kamm

Eagle
-------
Contains some cheap DIY boards i've used. Follow components are modeled now:
- RXB6 wireless receiver module
- RXB8 wireless receiver module
- CC1101 wireless transceiver/receiver module
- MP1584 based dc/dc step-down module
- MP2482 based dc/dc step-down module
