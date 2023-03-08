# TurboNanza
An internal RGB, S-Video, Composite video and Audio modification for the Turbografx 16, PCEngine and CoreGrafx. As of Revision C, support has been added for audio from the Turbo Everdrive Pro by 

Design is KiCad format and all files necessary to open the design and have it fabricated are present within the archive.

![](/images/Board%20Render.jpg?raw=true "")

Installation Method (WORK IN PROGRESS!!):

## Step 1 - Remove the resistors for Luma, R-Y, B-Y, and Burst
### PC Engine
Remove resistors R134, R137, R138 and R141
![](/images/RevC%20-%20PCE%20Step%201%20-%20Resistors.png?raw=true "")

### TurboGrafx 16
Remove resistors R130-R132 and R134
![Step 1](/images/Assembly%20Step%201A.jpg?raw=true "Step 1")

### CoreGrafx 1/2
Coming Soon...

## Step 2 - Disconnect CVBS pin from original circuit
### PC Engine
Remove resistor R145 (20 ohms)

![](/images/RevC%20-%20PCE%20Step%202%20-%20CV%20Resistor.png?raw=true "")

### TurboGrafx 16
Remove resistor R127 (20 ohms)

![Step 2](/images/Assembly%20Step%202.jpg?raw=true "Step 2")

### CoreGrafx 1/2
Coming Soon...

## Step 3 - Install TurboNanza
### PC Engine
Solder the TurboNanza over the expansion port pins as shown.
![](/images/RevC%20-%20PCE%20Step%203%20-%20Board.jpg?raw=true "")

### TurboGrafx16
Solder the TurboNanza over the expansion port pins as shown.
![](/images/RevC%20-%20TG%20Step%203%20-%20Board.jpg?raw=true "")

### CoreGrafx 1/2
Coming Soon...

## Step 4 - Solder S-Video connections
### PC Engine
Solder wires from the points shown to the pads on TurboNanza
![](/images/RevC%20-%20PCE%20Step%204%20-%20SV%20Solder%20Points.png?raw=true "")

### TurboGrafx 16
Solder wires from the points shown to the pads on TurboNanza
![Step 3](/images/Assembly%20Step%203.jpg?raw=true "Step 3")

## Step 5 - Attach the DIN to the main board
### PC Engine
Scrape solder mask off of the area where the RF modulator resided. Align the DIN such that it JUST covers the front mounting hole of the RF port.

![](/images/Rev%20C%20-%20PCE%20Step%205%20-%20DIN.png?raw=true "")
