# Light-Following-Robot
A 2-wheeled, analog light-following robot built using a breadboard chassis and pure hardware logic (no microcontroller).

Components: 
-2x TT Motors
-2x TT Wheels
-1x Castor Wheel
-1x H-Bridge Motor Driver L293D 
-1x 5V Regulator LM7805
-2x Photoresistors/Light Dependent Resistors
-2x Resistors (1k ohm)
-6/8-AA battery Holder
-6/8AA batteries

How it Works: 
Sensors: The LDRS act as the 'eye' of the robot detecting light and decreasing its resistance, it's hooked up with a voltage divider using a resistor of 1k ohm (adjustable per preference). When no light falls on the LDRs, they have maximum resistance thus current is goes through the path with less resistance but when the LDR's resistance decreases, current goes through the LDRs path.

Movement: From the LDR current travels to the L293D driver that sends powers to the motors with rotate its wheels.

Power: A 6-8 AA battery pack provides raw power to the motors via Pin 8 (Power 2/Vcc2), while an LM7805 regulates the voltage to a steady 5V for the Pin 16 
(Power 1/Vcc1).

Key Features:
The breadboard is used as the chasis/frame making the robot simple yet powerful and works with charm.
In case of an AA battery holder of 8AA batteries when the builder only has 6 as an example, a wire of copper may be used to connect the 2 terminals of the gap in the battery holder.
The heavy battery holder is placed ON the chasis right above the 2 motors providing heavy weight torque but fast movement.

*IMPORTANT: Make sure that the L293D Pin 8 goes to the Battery Positive, but Pin 16 goes to the Output of the 7805. This keeps the driver from burning out*
