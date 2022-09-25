# TurboNanza
An internal RGB, S-Video, Composite video and Audio modification for the Turbografx 16.

Design is KiCad format and all files necessary to open the design and have it fabricated are present within the archive.

![](/images/AsssembledPCB.jpg?raw=true "")


For RGB and Audio portions, simply fit the PCB over the expansion pins and solder down, then connect the output pins for RGB, Sync and Audio Left/Right to the corresponding pins of your chosen output connector.

To add S-video, First pull the left leg of R130 out of circuit as shown in the picture below, and connect the resistor to ground. Then remove resistors R131, R132 and  R134). Leave the Plated Through Holes open. Grounding R130 grounds the base for the composite mixing NPN transistor through R133.
![Step 1](/images/Assembly%20Step%201A.jpg?raw=true "Step 1")


Next, pull the bottom leg of R127 out of circuit.
![Step 2](/images/Assembly%20Step%202.jpg?raw=true "Step 2")

Finally, solder your wires for Y (Luma), R-Y, B-Y, and Color Burst to the points on the bottom of the board as shown. Connect these wires to the "YI", "RY", "BY" and "BRS" pads on the TurboNanza, and solder bridge the jumper for "CV", which will send the remixed composite video to the "V" output pad on the TurboNanza.
![Step 3](/images/Assembly%20Step%203.jpg?raw=true "Step 3")
![Step 4](/images/Assembly%20Step%204.jpg?raw=true "Step 4")
