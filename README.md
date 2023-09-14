# Pica40 v2

Split keyboard with 40 keys using XIAO controllers.

_Pica pica - european (common) magpie_

####  🏭 _Extra PCBs available_ 
_I have some extras laying around, ping me on discord/reddit if interested (EU only)._ 💶

## Features

- 40 keys
- high profile (regular MX switches with hotswap sockets) or low profile (soldered low-profile ChocV2 switches)
- wired/wireless versions
- aggressive stagger
- slightly splayed for pinky columns

### Wired version

- XIAO RP2040 controller
- QMK firmware
- USB-C or TRRS connection between splits
- one rotary encoder (without click)
- status LED

### Wireless version

- XIAO nRF52840 BLE controller
- ZMK firmware
- two rotary encoders (without click, only master side encoder is currently supported by ZMK)
- on/off toggle
- battery connectors

## Photos

wired version with 3d printed case

![](./images/v2.1-top.jpg)
![](./images/v2.1-bottom.jpg)

wired/wireless versions with Choc V2

![](./images/full.jpg)

Pica40 family - ChocV2 with low profile keycaps, ChocV2 with MT3 keycaps, Pica40 v1 with MT3 keycaps, regular switches and hotswap sockets

![](./images/height.jpg)

## Firmware

- QMK - available in [main repository](https://github.com/qmk/qmk_firmware/tree/master/keyboards/pica40), also check [my fork](https://github.com/zzeneg/qmk_firmware/tree/feature/pica40/keyboards/pica40) for most recent updates. [Compiled file](firmware/qmk/pica40_rev2_zzeneg.uf2).
- Vial - [my fork](https://github.com/zzeneg/vial-qmk/tree/feature/pica40/keyboards/pica40). [Compiled file](firmware/vial/pica40_rev2_vial-zzeneg.uf2).
- ZMK - [Source code](https://github.com/zzeneg/zmk-config), [compiled left](firmware/zmk/pica40_left.uf2), [compiled right](firmware/zmk/pica40_right.uf2), [reset](firmware/zmk/settings_reset.uf2)

## Gerber files

- [PCB](gerbers/pcb.zip)
- [Bottom plate](gerbers/bottom.zip)

## Case files (STL - 3d printed, MX hotswap only)

All files are in [stl](stl) folder.

### Top:

![](./images/render-top.png)

- wired/wireless versions
- with and without encoders
- normal and thin versions (see bottom parts for difference)

### Bottom:

Thin version - just cutouts for all elements, as low as it can be. May be combined with normal top case and metal bottom plate for additional weight.
![](./images/render-bottom-thin.png)
Normal (with legs and without):
![](./images/render-bottom.png)

## Case files (DXF - for metal/acrylic)

- [Curved bottom for MX hotswap with 3D printed case](dxf/bottom-curved.dxf)
- [Bottom for soldered ChocV2](dxf/bottom.dxf)
- [MCU cover](dxf/cover.dxf)
- [MCU cover with encoder hole](dxf/cover-hole.dxf)

## Bill of materials

- PCBs
- 2 XIAO MCUs - [RP2040](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html) for wired version, [nRF52840](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) for wireless
- 40 SMD SOD-123 1N4148 diodes
- 1 or 2 EC11/12 rotary encoder with knob (diameter up to 20mm)
- _[MX hotswap version]_ 3d printed case (top and bottom, left and right - 4 files)
- _[MX hotswap version]_ 40 hotswap sockets
- _[MX hotswap version]_ [M2 standoffs](https://www.aliexpress.com/item/4001271908929.html) (4mm for thin, 5mm for normal), 3mm [M2 screws with flat head](https://www.aliexpress.com/item/4001248931159.html)
- _[MX hotswap thin version]_ [8x2mm magnets](https://www.aliexpress.com/item/1005002285176336.html) (optional)
- _[ChocV2 soldered version]_ FR4/metal/acrylic bottom plates, metal/acrylic MCU cover (optional)
- _[ChocV2 soldered version]_ 6mm M2 screws, M2 nuts and washers
- _[Wired only]_ [USB-C 16pin connectors](https://www.aliexpress.com/item/1005003670899595.html)
- _[Wired only]_ [TRRS PJ-320A connectors](https://www.aliexpress.com/item/1005001928651798.html)
- _[Wireless only]_ [2x on/off toggle MSK-12C02](https://www.aliexpress.com/item/4000685483225.html)
- _[Wireless only]_ 2x Li-Ion 3.7V battery (up to 25x14x5 for standard case)
- Rubber [sheet](https://www.aliexpress.com/item/1005003938672544.html) or [5x15 legs](https://www.aliexpress.com/item/1005004431841328.html)

## Build log

**TODO**

## Changelog

### V2.1

- added TRRS support
- wired version supports rotary encoder on any side
- remove unused for FR4/acrylic/metal sandwich case, 3D printing is better and cheaper
- improved 3D printed case with a new shape and parts

### V2

- reworked to true split with two XIAO MCUs controllers
- added splay to pinky columns
- all case/pcb files are not compatible with V1

### V1

- split with single Pro Micro based MCU and handwired connection

## Support
If you like my work and want to support my future designs, please consider [sponsorship](https://github.com/sponsors/zzeneg).
