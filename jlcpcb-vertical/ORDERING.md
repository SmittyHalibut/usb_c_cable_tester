# Ordering Instructions for v3.0 boards on [JLCPCB](https://jlcpcb.com/) — vertical variant

This is the v3.0 design with **vertical connectors** and through-hole parts where possible,
intended for assembly by JLCPCB.

TODO 2026-06-16: Update images with v3.0 boards and process.

## Generate Files
This directory contains the KiCad source only. Generate the manufacturing files from
`usb_c_cable_tester.kicad_pcb` in this folder:

* **Gerbers** — KiCad PCB editor → *File → Plot* → Gerbers, then *Generate Drill Files*
* **BOM** + **Positions** — *File → Fabrication Outputs* (or the Fabrication Toolkit plugin)

Pre-built v3.0 production bundles (gerber zip, `bom.csv`, `positions.csv`) are attached to
the [v3.0 release / `jlcpcb` branch](https://github.com/alvarop/usb_c_cable_tester) if you'd
rather not regenerate them.

## Upload Gerbers and Select PCB Parameters
Go to JLCPCB, click on "instant quote" or "order now" and upload the gerber zip.

Select the following settings (or change how you like them)
* ENIG will look better, but it's a bit more expensive. I definitely recommend lead free HASL at the very least
* The image shows 0.8mm board thickness, but that is no longer necessary with v3.0 boards.  Use the default 1.6mm boards.
* Choose your color, it's free.  :-)

![Selection page](../img/1.png)

Make sure you select PCB Assembly as well then click Next

# Upload BOM and Placement files

This image shows old file names.  Upload the `bom.csv` and `positions.csv` you generated/downloaded earlier.

![Upload BOM](../img/2.png)

Verify BOM.  The parts have changed since this image. The important part to verify is that all parts are available and selected.  If a part is no longer available, you'll have to find a suitable replacement.

![BOM](../img/3.png)

## Fix Component Placement
Verify component placement (it's not quite right by default).  These images show v2.2 boards, and v3.0 looks different.  However, the concepts are the same:  Rotate and move parts so that the pins line up in the holes correctly.

First, rotate the battery holder 90 degrees to the left
![component placement](../img/4.png)
 
Then select each USB connector and use the arrows on the top right to move it into place
![front of board](../img/5.png)

You can change the view to the back to make sure the pins line up

![back of board](../img/6.png)

The 3d view is also quite useful when trying to line things up

![3d view](../img/7.png)

## Checkout!

![Checkout!](../img/8.png)

## Additional Notes
[There have been reports](https://github.com/alvarop/usb_c_cable_tester/issues/15) of JLC asking if all the pins on one side should be shorted together. The answer is yes, this is on purpose :D
