# 5-Axis-3D-Printer-Config
Reprap firmware config file for Auburn University 5 Axis 3D Printer senior design project.

When you boot up the printer, ensure the raspberry pi and the duet board are recieving power (LEDs should be on)
The Pi should boot into a desktop and auto-launch a web browser to open the web controller. 
If this browser claims no internet access, close it and open a new browser using the blue circle button in the top left, then select the Web Controller from the shortcuts in the browser

A-Axis is the mandrel (rotation about the x-axis)
B-Axis is the printer head rotation (

To change microstepping, open the config file and change the values in the M350 command. 

Ex: M350 X1 Y1 Z1 A1 B1 E16 I1

would set X, Y, Z, A, and B to have full stepping and E to have 1/16 microstepping

1 = full step
2 = half step
4 = quarter step
8 = 1/8 step
16 = 1/16 step
64 = 1/64 step
128 = 1/128 step
256 = 1/256 step