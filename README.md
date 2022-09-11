# TurboNanza
An internal RGB, S-Video, Composite video and Audio modification for the Turbografx 16

For RGB and Audio portions, simply fit the PCB over the expansion pins and solder down, then connect the output pins for RGB, Sync and Audio Left/Right to the corresponding pins of your chosen output connector.

To add S-video, First pull the left leg of R130 out of circuit as shown in the picture below, and connect the resistor to ground. Leave the Plated Through Hole open.
![Step 1](/images/Assembly%20Step%201.jpg?raw=true "Step 1")


Next, pull the bottom leg of R127 out of circuit.
![Step 2](/images/Assembly%20Step%202.jpg?raw=true "Step 2")

Finally, solder your wires for Y (Luma) and C (Chroma) to the points on the bottom of the board as shown. Connect these wires to the "Y_IN" and "C_IN" pads on the TurboNanza, and solder bridge the jumper for "CV", which will send the remixed composite video to the "V" output pad on the TurboNanza.
![Step 3](/images/Assembly%20Step%203.jpg?raw=true "Step 3")

