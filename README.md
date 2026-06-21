# USB Cable Tester

Simple board to test various USB cables! (Note the USB standard helps to identify these [USB-C](https://www.usb.org/usb-type-cr-cable-and-connector-specification), cables that are compliant with the standard will have selected pins according to [cable and connector specification release](https://www.usb.org/sites/default/files/USB%20Type-C%202.2%20Release%20202210%20%281%29.zip)). 

Plug in your cable to both sides and see which signals light up!

**FOR CABLE USE ONLY. DO NOT EVER PLUG THIS IN TO A DEVICE, THE PINS ON ONE SIDE ARE ALL SHORTED TOGETHER AND THAT COULD BREAK IT!**

![Board Front](img/front.jpg)

![Board Back](img/back.jpg)

## Board Variants

There are three variants of the board, each living in its own directory with the KiCad
source and ordering instructions. Pick the one that fits how you want to build it:

| Variant | Folder | Best for | Ordering |
|---------|--------|----------|----------|
| **Hand-solder** | [`hand-solder/`](hand-solder/) | DIY builds — through-hole-friendly parts from Digikey/Mouser, easy to solder and rework | [ordering](hand-solder/ORDERING.md) |
| **JLCPCB SMD** | [`jlcpcb-smd/`](jlcpcb-smd/) | Cheapest fully-assembled boards using current JLCPCB stock | [ordering](jlcpcb-smd/ORDERING.md) |
| **JLCPCB vertical** | [`jlcpcb-vertical/`](jlcpcb-vertical/) | Newest design (v3.0) — vertical connectors, through-hole where possible | [ordering](jlcpcb-vertical/ORDERING.md) |

Each folder is a self-contained KiCad project — open the `.kicad_pro` inside it.

## Related Projects!
@coryalder made a neat [3d printed/laser cut case](https://github.com/coryalder/usb-c-tester-case). Check it out! (But make sure it's for the correct version, since components have changed)

[@foorschtbar@chaos.social](https://mastodon.social/@foorschtbar@chaos.social) made a really nice 3D printed case (multicolor). You can [find it here.](https://www.printables.com/model/1003847-usb-cable-tester-multicolor-case)

## License
USB Cable Tester © 2024 by Alvaro Prieto is licensed under CC BY 4.0. To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/

The v3.0 (vertical) variant includes modifications © 2026 by Mark Smith, Halibut Electronics Inc. Same license applies.
