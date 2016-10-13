Arduino car tachometer
==============

Introduction
----
I'm currently driving an old Opel Astra without tachometer. I had a spare arduino and few LEDs, so I made a simple tachometer. I started by cut a 5cm x 1.5cm piece of an old credit cart, drilled 4 holes in it, painted it black and glued 4 LED diods to it. Then I soldered a 220ohm resistors to each positive LED pin and used a common ground. I connected them to arduino via 5x30cm jumpers and hid the arduino in a hole under the wheel. I connected the arduino data pin via voltage divider to the signal pin of the coil and used an old phone charger to power the arduino. In order to work I shared the phone charger and arduino's grounds.

The first LED turns on when engine react 4000 rpm. Below 4000 rpm all LEDs are turned off. If there is Serial attached, it automatically emits rpm data(watch it realtime in arduino serial monitor).

Demo
----

[Link to youtube video](https://www.youtube.com/watch?v=l8S7WWx-YB4&feature=youtu.be)

[![Arduino tachometer demo](http://img.youtube.com/vi/l8S7WWx-YB4/0.jpg)](http://www.youtube.com/watch?v=l8S7WWx-YB4)

Schematic
----
![Schematic](https://raw.githubusercontent.com/deepsyx/arduino-tachometer/master/Schematic.png)

Code
----
Check out the `code.cpp` file.

Materials
----
- Arduino Uno
- 4x LEDs
- 5x 220ohm resistor
- 1x 160ohm resistor
- 10x 30cm jumpers
- Old car phone charger
- Longer wire to connect to coil
- 1amp fuse (not included in schematics)

Future ideas
----
- More LEDs
- Log data (to phone or sd card) for analysis
- Graphic visualization for phone
