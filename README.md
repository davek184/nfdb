# USB-C Daughterboard for Norbaforce 

For all models of the Norbaforce (also works with the Norbauer Data Pad). 

Features USB-C port, ESD protection, over voltage protection, CC1 & CC2 resistors to work with USB-C to C cables.  

Finishes on Norbaforces vary greatly.  They were designed for USB mini cables so it is possible a USB-C cable end may not fit depending a finish. In those cases a very light filing of the USB opening using a hobby file can enlarge the opening just enough for the cable.

_(Note there is one PCB that can have a connector for Realforce 1 OR Realforce 2 models)_

# Version No Keyboard Connector
![RenderNoConnector](https://i.imgur.com/EpWg2Wn.jpg)
<br><br><br>

# Version Realforce R1 
  ![RenderRF1](https://i.imgur.com/ppieA41.jpg)
* **Models:** 86U, 87U, 88U, 91U
* **PCB Connector:** LCSC: C265068
* **Cable:** EH to EH (2.5mm pitch), 4 pin, SAME direction, Length 6cm (shielding cable 13cm)

![RF1Pinnout](https://i.imgur.com/Yg8DMYr.png)
<br><br><br>

# Version Realforce R2 
  ![RenderRF2](https://i.imgur.com/hHAMaGG.jpg)
* **Models:** R2 TKL, R2 RGB TKL, RT1 (numpad)
* **PCB Connector:** LCSC: C69152
* **Cable:** PH to PH (2.0mm pitch), 5 pin, REVERSED Direction, Length 11cm

![RF2Pinnout](https://i.imgur.com/rXatLpw.png)
<br><br>

# Manufacturing
<details>
  <summary>Details</summary>
* Manufacturing files are set up for JLCPCB. 
* Thickness does not matter suggest standard 1.6mm 
* "Remove Order Number" option choose "Specify Location" (uses "JLCJLC" on silkscreen for order # position)
* Assemble top side
* Choose assembly file version (No connector: need to solder then yourself, RF1 or RF2 as indicated above in renders)
* Manual part adjustments from KiCad Outputs (already handled in manufacturing files)

| Part              | Adjustment   |
| ----------------- | ------------- |
| USB-C Connector   | Down 5.06mm   |
| JST EH Connector  | Up 3.75mm   |
| JST PH  Connector | Rotate 90°, Down 4mm |

## BOM

| LCSC part # | Description      | Value | Package  | Amount |
| ----------- | ---------------- | ----- | -------- | ------ |
| C261942     | Fuse             |       | 0805     | 1      |
| C7519       | ESD              |       | SOT23-6  | 1      |
| C212411     | Resistor         | 5.1K  | 0805     | 2      |
| C597300     | Capacitor        | 4.7nF | 0805     | 1      |
| C165948     | Connector (USB)  |       | TH       | 1      |
| C265068     | Connector (EH)   | 4 pin | TH       | 1      |
| C69152      | Connector (PH)   | 5 pin | TH       | 1      |

_Note if the capacitor or resistors are out of stock they can be replaced with 0805 sized component with similar specs._
</details>

# EH -> PH Cable Experiments
<details>
  <summary>Details</summary>
Tested a sample cable using manufactured PH crimped wires in an EH cable housing end (LCSC: C161661) to make a PH to EH cable without manually crimping.  Worked without issues after 350 connection cycles.  Potential could use R2 daughterboard connector can be used for both R2 and R1 boards.

![CableEHToPH](https://i.imgur.com/tfvrSqY.png)
</details>

# Notes
<details>
  <summary>R2 NFDB and the Realforce RT1 (Topre numpad)</summary>

The R2 NFDB is compatible with the Topre Realforce RT1 numpad (released in 2024), which shares a similar footprint to the predecessor Realforce 23u.  
![RT12](https://i.imgur.com/HHpbOw6.jpeg)

</details>  
<details>
  <summary>Photos</summary>

Norbaforce MKI (cutout is USB shape no issues with fit)
![NFMKI](https://i.imgur.com/Zcj5vSL.jpg)
Norbaforce MKIII (unfinished no fit issues)
![NFMKII](https://i.imgur.com/ojrkUOl.jpg)
Norbaforce MKII RF2
![NFMKiib](https://i.imgur.com/GUCTGYN.jpeg)
Norbaforce MKII (slight internal filing was needed)
![NFMKIIInside](https://i.imgur.com/2XnP7rR.jpg)
Norbauer Data Pad and the R1 NFDB
![DataPad](https://i.imgur.com/ypJBltZ.jpg)
Norbauer Data Pad with RT1 pcb - use R2 NFDB
![RT1](https://i.imgur.com/QSRFrbK.jpeg)
</details>

# Special thanks 
* Nekotato: for requesting, testing & driving this project
* Techbeezin: for test fitting the vast collection of Norbaforces 
* Cipulot: answering various questions regarding Realforce and general electrical questions/advice
* d0nk: for pre-testing the R2 OEM cabling/pinout on RT1
