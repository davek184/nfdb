# USB C Daughter/Breakout board for Norbaforce 

For the Norbaforce (MK1 fits perfect, MK2 & MK3 have small USB openings for USB-C connector but it does fit).  Features ESD protection, over voltage protection, CC1 & CC2 resistors to work with USB-C to C cables.  There are 2 daughterboard PBCs in this design to save money when manufacturing and since the Norbaforce can support both makes more sense to do it this way then one PCB design per type.

![Front](https://i.imgur.com/rTF9m1T.png)
![Back](https://i.imgur.com/VAFtKtq.png)

## R1 Realforce: JST EH connector
* Keyboards: R1 RealForces 86U, 87U, 88U, 91U
* Cable: EH to EH (4 pin, 2.5mm pitch), Shielding cable 13cm 

## R2 Realforce: JST PH connector
* Keyboards: R2 TKL, R2 RGB TKL
* Cable: PH to PH  (5 pin, 2.0mm pitch) 11cm

## Production
Production files are set up for JLCPCB. 
* For the "Remove Order Number" option choose "Specify Location" (Places JLCPCB production number over the JLCJLC silkscreen see render)
* Assemble top side
* Part placement adjustments for JLCPCB (these are already set in production files but will need to be manually done again if new files are generated)

| Part              | Adjustment   |
| ----------------- | ------------- |
| USB-C Connector   | Down 5.06mm   |
| JST EH Connector  | Up 3.75mm   |
| JST PH  Connector | Rotate 90°, Right ~0.3mm |

## BOM

| LCSC part # | Description   | Value | Package  | Amount |
| ----------- | ------------- | ----- | -------- | ------:|
| C261942     | Fuse          |       | 0805     | 2      |
| C7519       | ESD           |       | SOT23-6  | 2      |
| C212411     | Resistor      | 5.1K  | 0805     | 4      |
| C21217      | Capacitor     | 4.7nF | 0805     | 2      |
| C165948     | Connector     |       | TH       | 2      |
| C265068     | Connector (EH)| 4 pin | TH       | 2      |
| C265104     | Connector (PH)| 5 pin | SMT      | 2      |

_Note if the capacitor or resistors are out of stock they can be replaced with 0805 sized component with similar specs._

## Revisions
1.0
* Initial prototype

1.1
* Updated Design so that both RF1 & RF2 models can be printed in one file (saves money when manufacturing). 
* Flipped silkscreen orientation for those with a clear case.  
* Minor trace routing and silkscreen adjustments.
* Updated JST PH connector to surface mount instead of through hole.
