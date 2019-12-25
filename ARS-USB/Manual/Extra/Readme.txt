Generic controller with ARS-USB 
===============================

Through the ARS-USB Unit and with few additional components, can perform a motor controller.

You have to distinguish two possible types of controllers, depending on the type of tension that use the motor:

A.- AC Voltage
--------------
It is most common to find and are like most rotators work, eg G250, G450, G650, HAMiV, T2X.
These rotators need 3 wires and a capacitor (C) for starting. Some motors include this Capacitor inside the controller,
in which case to replace the original controller, you will get one to be used with ARS-USB.
Furthermore, most rotators usually use a 24VAC power.

Then in short, AC engines need to add to ARS-USB:
- A 100uF capacitor connected between 2 of the 3 wires that go to the electric motor.
- Source or transformer that delivers 24Vac. 


B.- DC Voltage
--------------
Example of this type of rotator we have it in the Prosistel Series "D" or Yaesu G800/G1000.
In this case, it is not necessary the capacitor, and 2 wires are used only to the motor.
By applying a voltage "V" (V depends on the type of motor) rotates in one direction and in the opposite reverse V.
Generally, as AC motors, typically operate at 24V, although there are motors, such as Prosistel, using 12Vdc.

C.- Antenna Position
--------------------
Finally, the position is obtained by means of a potentiometer (POT) having the external rotator and that drive the motor, 
is changing its resistance.

If one of the legs of the POT is connected to ground and put the other to 5VDC (could also be used 12Vdc) when the rotator changes the 
potentiometer from a limit (left) to the other (right), we get in the POT cursor a voltage between 0V and 5Vdc. This feedback will be
used by the ARS-USB to determinate the antenna position.

The ARS-USB can supply 5Vdc on the right pin of the 7805 regulator (IC5) close to J3.
We have a ground point available on pin 3 (central) J4 input. Remember to connect J4-3 to J4-4 (common ground). 
The feedback voltage is connected to J4-5.


