# What is this?

A minimalistic 3d printer toolhead design, build from ground up for tool changing and primarily the Voron Family of printers.
Inspired by [Tapchanger](https://github.com/viesturz/tapchanger) and [Stealthchanger](https://github.com/DraftShift/StealthChanger). But not getting into  [PitStop](https://mihaidesigns.com/pitstop3/) territory yet.

![Preview](./Images/Main.jpg)

## How is this different?

ClickChanger is a yet another vertically attached design, but building on previous experiences, but here are some design directions it focuses on:
* A hotend based nozzle probe, like Revo PZ, not requiring the smooth vertical movement by the docking mechanism
* Rigid connection between the Y rail and hotend's heatsink, minimizing thermal expansion differences between toolheads
* A Shared part cooling fan integrated in the shuttle, connected via Pogo pins
* A "naked" toolhead, allowing for better cooling and overall less weight.

And keeping the features from other designs:

* Vertical motion to attach/detach the toolhead
* No wires to the shuttle, single cable to each toolhead

# This is a Beta

This is still in testing, instructions are being worked on, only a few extruders/hotends are supported.

See [TapChanger](https://github.com/viesturz/tapchanger) for my docking/wiring setup.

See [Klipper-Toolchanger](https://github.com/viesturz/klipper-toolchanger/) for klipper firmware, [example config](https://github.com/viesturz/klipper-toolchanger/tree/main/examples/probe%20on%20T0).

### Roadmap

Some of next directions this is going, in no particular order

* Documentation documentation documentation
* Get to 1000+ toolcahanges without fail

### Contributing

Please file bugs and pull requests. My free time is quite limited, so will answer irregularly.
[Voron Toolchangers Discord](https://discord.com/invite/xmDWrYGwVJ) has lots of toolchanger users.
Also check out the [Youtube channel](https://www.youtube.com/playlist?list=PLqU7kX5nUJDT31KPcYAykZ2nuPKu_lhjn).

# Supported hotends

* Revo Voron
* Dragon or Dragon High flow
* Rapido HF (not the UHF)

# Supported extruders

* HGX Large Gears - personal favorite of mine, great for flexibles; lowest weight and integrated strain relief.
* HGX Large Gears V2
* Orbiter V2
* Sherpa mini and compatibles

# Supported toolboards
* Bitgtreetach EBB36 and compatibles
* Mellow Fly SHT36 V2 and Pro
* LDO Nitehawk (untested)

# BOM

**Common consumables**

* M3 screws, button head preferrably, 8mm and some other sizes
* M3x5x4 heatset inserts (voron spec)
* superglue, small tip tube, low viscosity

**Shuttle**

* 2x 4x12mm rounded end steel pins
* 1x 4x6x6mm bushing; preferrably the hybrid bushings for smoother slide
* 1x 3x8mm steel pin
* 1x 3x6x2.5mm bearing (3x6x3 works too)
* 1x 4010 centrifugal fan; 15000 rpm recommended since you are running a single fan.
* 2x 6x3mm magnet

**Shuttle CPAP**

* a CPAP fan
* ~1m 15mm diameter tube
* a 3x6x2.5mm bearing (3x6x3 works too)
* a 2gram micro servo, DSPOWER has worked well for me
* 2 m2x6 screws
* some servo wire

**Toolhead**

* A supported extruder, toolhead, toolboard
* 1x 4mm x12mm round end steel pins
* 2x 4x6x6 mm bushing; preferrably the hybrid bushings for smoother slide
* a Omron D2F-F limit switch or compatible
* 30x30x10 or 30x30x7 axial fan for hotend cooling
* 1x m2x6 **socket head** screw
* 4x 6x3mm magnets
* 2x 3.5mm [pogo pin](https://www.aliexpress.com/w/wholesale-pogo-pin-3mm.html), not needed for CPAP

**Dock**

* 30 mm of 7x0.1mm springsteel, salvageable from 1m tape measure.
* High temp silicone for the nozzle pad
* 2x 6x3mm magnets

# Assembly instructions

Coming up

# Revision log

## 1.1 - CPAP edition

* CPAP and eddy current probe support.
* Docks slightly redesigned, added magnets in docks.

![CPAP](./Images/CPAP.jpg)}


## 1.0 - Fingers crossed

The first one that is ready to be beta tested. **Not compatible with previous ones** the shuttle interface has changed.

Added: 
* Rigid mount dock initial version
* CPAP initial version

Small refinements across the board


## 0.9 - Small improvements

Added:

* Rapido extruder base
* Nitehawk toolbard cage

Small refinements across the board:

* HGX Lite gears 2 refinements
* Fan shroud refinements
* Better fit for some holes


## 0.8 - It prints!

Introduced pogo pins for the fan connection and a new wiring holder.

Full PTFE tube channel for HGX - better for flexibles.

Assembly is quite repeatable now.

Printing reasonably stable now, hundreads of toolchanges but still expect some warts.

![Pogo pins](./Images/Pins.jpg)

## 0.1 - It clicks!

There is an initial BOM, the click force is good, assembly is repeatable, building two and putting to the test.

![Toolheads](./Images/Toolheads-0.1.jpg)
![Shuttle](./Images/Shuttle.jpg)
