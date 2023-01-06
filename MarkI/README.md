# USB C Daughter/Breakout board for Norbaforce 

![Front](https://i.imgur.com/3oGNONb.png)
![Back](https://i.imgur.com/yq24EKO.png)

The Mark I Norbaforce is only compatible with the RealForce R1 keyboards.  (Kept the R2 connector on the daughterboard incase someone changes that in the future)

## R1 Realforce: JST EH connector
* Keyboards: R1 RealForces 86U, 87U, 88U, 91U
* Cable: EH to EH (4 pin, 2.5mm pitch), Shielding cable 13cm 

## Production
Production files are set up for JLCPCB. 
* For the "Remove Order Number" option choose "Specify Location" (Places JLCPCB production number over the JLCJLC silkscreen see render)
* Assemble top side
* Part placement adjustments for JLCPCB (these are already set in production files but will need to be manually done again if new files are generated)

| Part              | Adjustment   |
| ----------------- | ------------- |
| USB-C Connector   | Down 5.06mm   |
| JST EH Connector  | Up 3.75mm   |

## BOM

| LCSC part # | Description   | Value | Package  | Amount |
| ----------- | ------------- | ----- | -------- | ------:|
| C261942     | Fuse          |       | 0805     | 1      |
| C7519       | ESD           |       | SOT23-6  | 1      |
| C212411     | Resistor      | 5.1K  | 0805     | 2      |
| C21217      | Capacitor     | 4.7nF | 0805     | 1      |
| C165948     | Connector     |       | TH       | 1      |
| C265068     | Connector (EH)| 4 pin | TH       | 1      |
| C69152      | Connector (PH)| 5 pin | TH       | 1      |

_Note if the capacitor or resistors are out of stock they can be replaced with 0805 sized component with similar specs._

## Revisions
1.0
* Initial prototype

1.1
* Flipped silkscreen orientation
* Minor trace routing and silkscreen adjustments
