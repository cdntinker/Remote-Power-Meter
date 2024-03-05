## The Jacks
* J1 Power / Communications
* J2 Source connection for USB
* J3 Source connection for whatever
* J4 Source connection for whatever
* J5 Load connection for USB
* J6 Load connection for whatever
* J7 Load connection for whatever
* Disp1 Little OLED screen

## JP1 & JP2
These allow 4 of the possible 16 addresses for the INA219 chip.

The chip allows for 16 addresses by tying A0 & A1 to GND, VS+, SCL & SDA is various conbinations but I don't feel that much chaos is warranted in this case.

## R1 & R2
These are the shunt resistor that the INA219 uses for measuring current. There are 2 resistors in parallel to improve power handling (& possibly accuracy). 

A 2816 SMD resistor can typically handle ~2W and the initial design incentive is a device capable of supplying 4W.

## The LEDs
D1 is for indicating connection status.

D2 is intended to show alerts & such at a glance.

JP3 is just there to allow for driving the LEDs from either raw 5v (from the USB supply) or 3v3 (from the regulator).

