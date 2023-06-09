# TurboNanza
An internal RGB, S-Video, Composite video and Audio modification for the Turbografx 16, PCEngine and CoreGrafx. As of Revision C, support has been added for audio from the Turbo Everdrive Pro by 

Design is KiCad format and all files necessary to open the design and have it fabricated are present within the archive.

![](/images/Board%20Render.jpg?raw=true "")

Installation Method (WORK IN PROGRESS!!):

## Step 1 - Remove the resistors for Luma, R-Y, B-Y, and Burst
### PC Engine & CoreGrafx
~~Remove resistors R134, R137, R138 and R141~~

Remove resistors R134, R137, R138 and R156 

![](/images/RevC_PCE_Step_1.jpg?raw=true "")

### TurboGrafx 16
Remove resistors R130-R132 and R134
![Step 1](/images/Assembly%20Step%201A.jpg?raw=true "Step 1")

### SuperGrafx
Remove resistors R164-167
![Step 1](/images/RevC_SG_Step_1_Resistors.jpg?raw=true "Step 1")


## Step 2 - Disconnect CVBS pin from original circuit
### PC Engine & CoreGrafx
Remove resistor R145 (20 ohms)

![](/images/RevC%20-%20PCE%20Step%202%20-%20CV%20Resistor.png?raw=true "")

### TurboGrafx 16
Remove resistor R127 (20 ohms)

![Step 2](/images/Assembly%20Step%202.jpg?raw=true "Step 2")

### SuperGrafx
Remove resistor R147 

![Step 2](/images/RevC_SG_Step_2_CV_Resistor.jpg?raw=true "Step 2")

## Step 3 - Install TurboNanza
### PC Engine & CoreGrafx
Solder the TurboNanza over the expansion port pins as shown.
![](/images/RevC%20-%20PCE%20Step%203%20-%20Board.jpg?raw=true "")

### TurboGrafx16
Solder the TurboNanza over the expansion port pins as shown.
![](/images/RevC%20-%20TG%20Step%203%20-%20Board.jpg?raw=true "")

### SuperGrafx
Prepare the flex cable by tinning the pads as shown.

![Step 3A](/images/RevC_SG_Step_3A.jpg?raw=true "Step 3A")

Solder the TurboNanza to the flex cable as shown. It's recommended to verify continuity. Place some kapton/polyimide tape over the exposed solder pads on the bottom of the flex cable to avoid shorting to the shielding.
![Step 3B](/images/RevC_SG_Step_3B.jpg?raw=true "Step 3B")

Solder the TurboNanza/Flex Cable combo over the expansion port pins as shown (ignore 4 wires at this time).
![Step 3C](/images/RevC_SG_Step_3C.jpg?raw=true "Step 3C")

## Step 4 - Solder S-Video connections
### PC Engine & CoreGrafx
Solder wires from the points shown to the pads on TurboNanza
(Do not remove R141, as previously directed. The Color Burst trace runs underneath and can easily sever. Leave R141 on and solder directly to the resistor pad)

![Step 4](/images/RevC%20-%20PCE%20Step%204%20-%20SV%20Solder%20Points.png?raw=true "")

### TurboGrafx 16
Solder wires from the points shown to the pads on TurboNanza
![Step 4](/images/Assembly%20Step%203.jpg?raw=true "Step 3")

### SuperGrafx
Solder wires from the points shown to the pads on TurboNanza
![Step 4](/images/RevC_SG_Step_4.jpg?raw=true "Step 4")

## Step 5 - Attach the DIN to the main board
### PC Engine
Scrape solder mask off of the area where the RF modulator resided. Align the DIN such that it JUST covers the front mounting hole of the RF port.

![](/images/Rev%20C%20-%20PCE%20Step%205%20-%20DIN.png?raw=true "")

### CoreGrafx
Using the supplied mounting board, mount using the ground plated through holes for the original DIN. Align the DIN on the mounting board such that it aligns with the console shell opening and solder in place.

Pictures Forthcoming


### TurboGrafx16
Solder the mounting board using the plated through holes for the RF modulator. Align the DIN on the mounting board such that it aligns with the console shell opening and solder in place.

![](/images/RevC_TG_Step5_DIN.jpg?raw=true "")

## Step 6 - RF Shielding and Case trimming
### PC Engine
On the bottom shell of the case, trim the 2 ribs where the expansion port opening sits. Do not re-install the original shielding.

### CoreGrafx
Trim the RF shield such that the metal lip is not contacting the TurboNanza.

![](/images/RevC_CG_Step6_RFShield.png?raw=true "")

Like the PC Engine, trim the 2 ribs on the bottom shell where the expansion port opening is.
