# Electronics documentation
**Tools needed:**

- TODO

**Content:**

[TOC]

Note:

The [hackaverde project](https://github.com/PostalBlab/hackaverde/tree/master/images) also has some high quality images of the PCBs including the front panel.

## power supply box

After disassembly we saw a power distribution box on the water-reservoir side.

It has outputs

* Output-N - thick blue cable - to electronics box
* OP-N1 - thick blue cable - to water heater
* OP-N2 - thick white cable - to 700W roasting lamp (other think white cable comes from electronics box)
* OP-N3..N5 - front panel electronics (?)
* OP-N5 - 2 thin yellow cables - to roasting turntable
* OP-N6 - thin black - to electronics box



<img src="..\Bonaverde_disassembly\opened_left.JPG" alt="opened_left" style="zoom:12%;" />

<img src="..\Bonaverde_disassembly\opened_power_electronics_box.JPG" alt="opened_power_electronics_box" style="zoom:12%;" />

## relay box

<img src="..\Bonaverde_disassembly\opened_right.JPG" alt="opened_right" style="zoom:12%;" />

The box has a screw on the bottom of the side and 2 obvious push fit connectors.
It can be opened without detaching the front panel.
It seems to get lower power signals from the front panel and switch the different high power elements.
So it seems like we can attach ourself to that ribbon cable instead of the front panel to control this machine without having to touch any high power electronics ourself.

### CN21

This connector seems to be our power supply for the front panel.
It should also serve as a nice power supply for our new Raspberry Pi.

* Black = GND
* White = -5V
* Red = -24V

### CN9

This 10x2 ribbon cable seems to do contain all the control signals we need to attach to.

* TODO: map out the pins
* 1 (PCB side left)
* 2
* 3 (PCB side 2nd from left)
* 4 
* 5 (PCB side 3rd from left)
* 6 
* 7 (PCB side 4th from left) - Micro switch for inserted coffee pot  - pulled to GND
* 8 - +3,3V supply?
* 9 (PCB side 5th from left)
* 10
* 11 (PCB side 6th from left)
* 12 - Micro switch for roast tray being inserted  - pulled to GND
* 13 (PCB side 7th from left) - Micro switch for inserted air filter  - pulled to GND
* 14 - +5V supply?
* 15 (PCB side 8th from left)
* 16 - +3,3V supply?
* 17 (PCB side 9th from left)
* 18 -
* 19 (PCB side rightmost one)
* 20 - some +3,3V signal (3,21V when idle)

### less interesting ones:

#### SW7

Switch for the air-filter door

...

#### ACL

Power input from the power supply box (Brown)

#### CN1

Stepper(?) motor for roasting fan

#### CN2

Power output to the water heater

#### CN4

* 1+2 (Red) **Unknown** - first small Sensor(?) PCB below roasting chamber
* 3+4 (Black) **Unknown** - second small Sensor(?) PCB below roasting chamber
* 5+6 (Brown) Micro switch in roasting chamber

#### CN5

Power input from the power supply box (White)

#### CN6

Micro switch for inserted coffee pot (2x Black)

#### CN7

230V 4W motor to open door below grind (White)

#### CN10

Unknow to coffee pot heater plate (White)

#### CN14

Tap to the water-heater power. 
(Thick blue cables connected to OP-N1 in the power supply box)

#### CN15-1

Roasting turntable motor (blue)

#### CN15-2

Roasting turntable motor (black)

#### CN16-1

Power input from the power supply box (Blue)

#### CN17

**Unknown** (White)

#### CN18-1

230V 6W grinder motor (Black) 

#### CN18-2

230V 6W grinder motor (Red)

#### CN20

Unused

#### NTC1

**Unknown** (Brown)

#### NTC2

Roasting chamber temperature probe (White)

## Front panel

TODO...
