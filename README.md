# USB C Daughter/Breakout board for Norbaforce

EST and over voltage protection.  CC1 & CC2 resistors to work with USB-C to C cables.

## JST EH connector (4 pin):
TODO: Photo close up

## JST PH connector (5 pins): 
TODO: Photo close up

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

## Production
Production files are set up for JLCPCB.  There were a few postion tweaks for connectors vs what KiCad generates.  Note there are 3 different versions depending on the connector choosen EH, PH or none (self solder the appropriate one)

## Revisions
1.0 Initial prototype

1.1 Flipped silkscreen orientation.  Minor silk screen adjustments for readability.
