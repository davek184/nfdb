# USB C Daughter/Breakout board for Norbaforce 

For the Norbaforce Mark II & Mark III (no idea on Mark I).  Features ESD protection, over voltage protection, CC1 & CC2 resistors to work with USB-C to C cables.  These PCB design is the same daughterboard stamped out twice for R1 realforces (EH connector) & R2 Realforces (PH connector).

[TODO: Combined photo]

## R1 Realforce: JST EH connector (4 pin, 2.5mm pitch):
Realforce Boards using this connector: R1 RealForces 86U, 87U, 88U, 91U
[TODO: Photo close up]

## R2 Realforces: JST PH connector (5 pins, 2.0mm pitch): 
Realforce Boards using this connector: R2 TKL, R2 RGB TKL
[TODO: Photo close up]

## Production
Production files are set up for JLCPCB.  There were a few postion tweaks for connectors vs what KiCad generates. 

## BOM

| LCSC part # | Description   | Value | Package  | Amount |
| ----------- | ------------- | ----- | -------- | ------:|
| C261942     | Fuse          |       | 0805     | 2      |
| C7519       | ESD           |       | SOT23-6  | 2      |
| C212411     | Resistor      | 5.1K  | 0805     | 4      |
| C21217      | Capacitor     | 4.7nF | 0805     | 2      |
| C165948     | Connector     |       | TH       | 2      |
| C265068     | Connector (EH)| 4 pin | TH       | 2      |
| C69152      | Connector (PH)| 5 pin | TH       | 2      |

## Revisions
1.0 Initial prototype

1.1 Flipped silkscreen orientation.  Minor silk screen adjustments for readability.
