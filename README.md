# TurboNanza
[PC Engine Shuttle Installation Instructions](/images/shuttle/readme.md)

[PC Engine/Turbo Duo Installation Instructions](/images/duo/readme.md)

An internal RGB, S-Video, Composite video and Audio modification for the Turbografx 16, PCEngine and CoreGrafx. As of Revision C, support has been added for audio from the Turbo Everdrive Pro by 

Design is KiCad format and all files necessary to open the design and have it fabricated are present within the archive.

![](/images/Board%20Render.jpg?raw=true "")

Installation Method (WORK IN PROGRESS!!):

PINOUT (For reference/Non-Expansion-Port Installs):
![](/images/Pinout.jpg?raw=true "")




## Step 1 - Remove the resistors for Luma, R-Y, B-Y, and Burst
### PC Engine & CoreGrafx

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

**When soldering the Y/B-Y/R-Y/Burst wires, try to use as close to the exact same length of wire as possible to maintain proper phase shift!**

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
Kits sold after 8/15/2023 now include a mounting board for the PCEngine. It is recommended to secure with two size M2 or 2-56 bolts/washers to allow for easy positioning.

Position the mount and loosely secure with screws/washers. The board may also be soldered - kapton/polyimide tape is recommended to position the board.
![](/images/PCE_Step5A.jpg?raw=true "")

Place the DIN in the slot, and solder around the sides.
![](/images/PCE_Step5B.jpg?raw=true "")

Solder the DIN FFC adapter to the DIN.
![](/images/PCE_Step5C.jpg?raw=true "")


Kits without mounting board: scrape solder mask off of the area where the RF modulator resided. Align the DIN such that it JUST covers the front mounting hole of the RF port.

![](/images/Rev%20C%20-%20PCE%20Step%205%20-%20DIN.png?raw=true "")

### CoreGrafx
First, remove C162 (AC coupling capacitor for composite video - no longer necessary)
![Step 5](/images/RevC_CG_Step5A.jpg?raw=true "Step 5")

Scrape the solder mask off the copper on the left and right edges of the original DIN footprint as shown.
![Step 5](/images/RevC_CG_Step5B.jpg?raw=true "Step 5")

Solder the supplied mounting board to the mainboard.
![Step 5](/images/RevC_CG_Step5C.jpg?raw=true "Step 5")

Due to the cartridge PCB coming into contact with the DIN-FFC board, follow this procedure. First, place the DIN-FFC board on the DIN without soldering.
![Step 5](/images/RevC_CG_Step5D.jpg?raw=true "Step 5")

Put everything together as if reassembling - this will allow the cartridge PCB to tilt the DIN-FFC PCB.
![Step 5](/images/RevC_CG_Step5E.jpg?raw=true "Step 5")

![Step 5](/images/RevC_CG_Step5F.jpg?raw=true "Step 5")

Finally, solder the DIN-FFC in the resulting position.
![Step 5](/images/RevC_CG_Step5G.jpg?raw=true "Step 5")


### TurboGrafx16
Solder the mounting board using the plated through holes for the RF modulator. Align the DIN on the mounting board such that it aligns with the console shell opening and solder in place.

![](/images/RevC_TG_Step5_DIN.jpg?raw=true "")

### SuperGrafx
Remove the original DIN and scrape the soldermask approximately as shown.
![](/images/RevC_SG_Step5A.jpg?raw=true "")

Solder the mounting board as shown, aligning the center hole with the two ground through holes.
![](/images/RevC_SG_Step5B.jpg?raw=true "")

Mount the DIN and DIN board to the mount board.
![](/images/RevC_SG_Step5C.jpg?raw=true "")


## Step 6 - RF Shielding and Case trimming
### PC Engine
On the bottom shell of the case, trim the 2 ribs where the expansion port opening sits. Do not re-install the original shielding. If your PC Engine has shielding that has two tabs that solder close to the EXP port pins, you will need to run a wire to where the shielding originally terminated.
![](/images/PCE_CG_Step6X.jpg?raw=true "")

![](/images/PCE_CG_Step6X2.jpg?raw=true "")


### CoreGrafx
Trim the RF shield such that the metal lip is not contacting the TurboNanza.

![](/images/RevC_CG_Step6_RFShield.png?raw=true "")

Like the PC Engine, trim the 2 ribs on the bottom shell where the expansion port opening is.


