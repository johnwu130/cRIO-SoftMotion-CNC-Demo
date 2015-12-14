# cRIO-SoftMotion-CNC-Demo
A CNC motion controller based on NI CompactRIO and SoftMotion

Purpose:
This demo demonstrates the ability for cRIO to act as a controller for general motion control and/or CNC control applications.  The FPGA code provided is a template for 5-axes open-loop motion control, complete with limit switch support.  This code also leverages my DXF Parser and GCODE Parser to interpret these files into the corresponding SoftMotion commands.  Sample DXF and GCODE files are also provided in the example.

Disclaimers:
1.	The DXF and GCODE Parser are only proof-of-concept examples.  They have not been extensively tested with all kinds of files.  This parsers are not meant to be complete SW products.
2.	This example code is also not meant to be a complete CNC controller solution.  There are many solid CNC controllers in the market today, such as Siemens and Fanuc.  Please do not give the customer the wrong expectations.

HW/SW Requirements:
•	cRIO-9033
•	NI 9401 x1 (For CW/CCW pulse output)
•	NI 9403 x1 (For home switches and enable signals)
•	Mini-displayport to VGA/DVI/HDMI converter and Monitor (res: 1920x1080)
•	3-axis gantry machine (such as CNC routers or 3D printers.) 
•	LabVIEW 2014, Real-Time, FPGA, and SoftMotion Modules
You can also run this code in pure PC simulation mode, if you do not have the HW.  This demo supports up to 5 axes of motion, but only 3 are used for this demo.  Code can be easily compiled for other targets.
