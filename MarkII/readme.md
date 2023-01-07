# USB C Daughter/Breakout board for Norbaforce 

For the Norbaforce (MK2) Features ESD protection, over voltage protection, CC1 & CC2 resistors to work with USB-C to C cables.  

There are 2 daughterboard PBCs in this design to save money when manufacturing and since the Norbaforce can support both.  Makes more economic sense to manufacture this way (yes could have been panelized more efficently, my first attempt at panelizing)

[TODO: Once samples arrive include photo with riser)

![Render](https://i.imgur.com/sFphkfc.png)

## R1 Realforce: JST EH connector
* Keyboards: R1 RealForces 86U, 87U, 88U, 91U
* Cable: 
  * EH to EH 2.5mm pitch
  * 4 pin
  * Lenth: 13cm 
  * SAME DIRECTION pinnout

## R2 Realforce: JST PH connector
* Keyboards: R2 TKL, R2 RGB TKL
* Cable: PH to PH  (5 pin, 2.0mm pitch) 11cm

## Production
* Production files are set up for JLCPCB.  
* For now only Gerber file is included
* For the "Remove Order Number" option choose "Specify Location" (Places JLCPCB production number over the JLCJLC silkscreen see render)
* Note only Gerber file is included now so part files would need to be generated from KiCad.  Inaddition this would need to be manually soldered for the USB raiser with pin headers

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
(Pin headers 2.54mm pitch)

_Note if the capacitor or resistors are out of stock they can be replaced with 0805 sized component with similar specs._

## Revisions
1.0
* Initial prototype

1.1
* Added usb riser section to better fit Norbaforce
* Updated Design so that both RF1 & RF2 models can be printed in one file (saves money when manufacturing)
* Flipped silkscreen orientation for those with a clear case.  
* Updated JST PH connector to surface mount instead of through hole.
