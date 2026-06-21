# Ordering & Assembly Instructions — hand-solder variant

This variant is designed to be **hand-assembled** with through-hole-friendly parts you can
buy from Digikey/Mouser. You order **bare boards only** (no PCB assembly) and solder the
components yourself, which makes the boards much cheaper.

## 1. Generate gerbers
This directory contains the KiCad source only. Open `usb_c_cable_tester.kicad_pcb` in this
folder and export gerbers: *File → Plot* → Gerbers, then *Generate Drill Files*. Zip the
output directory.

## 2. Order bare PCBs
Upload the gerber zip to any fab ([JLCPCB](https://jlcpcb.com/), OSH Park, etc.).

* Do **NOT** select PCB Assembly — order bare boards only.
* Lead-free HASL is fine; ENIG looks nicer if you want to spend a bit more.
* Pick any color, it's usually free.

## 3. Source components and solder
Populate the board by hand using the parts in the BOM (`usb_c_cable_tester_BOM.csv` /
`usb_c_cable_tester.xml` exported from the schematic). All parts are commonly available from
Digikey/Mouser.

## Additional Notes
[There have been reports](https://github.com/alvarop/usb_c_cable_tester/issues/15) of fabs
asking if all the pins on one side should be shorted together. The answer is yes, this is on
purpose :D
