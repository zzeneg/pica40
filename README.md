# Pica40 v2

Split keyboard with 40 keys using XIAO controllers.

_Pica pica - european (common) magpie_

## Features

- 40 keys - regular MX switches with hotswap sockets or soldered low-profile ChocV2 (with MX stem)
- wired/wireless versions
- aggressive stagger
- slightly splayed for pinky columns

### Wired version

- XIAO RP 2040 controller
- QMK firmware
- USB-C connection between splits
- rotary encoder on left side only (without click)
- one status LED

### Wireless version

- XIAO BLE controller
- ZMK firmware
- on/off toggle
- battery connectors

## ⚠️ Known issues

- wired version is not fully compatible with low profile ChocV2 switches, 1.5U keycap cannot be bottomed out because of USB-C connector - to be fixed in new revision

## Photos

<img src='images\full.jpg' width="600">
<img src='images\left.jpg' width="600">
<img src='images\right.jpg' width="600">
<img src='images\height.jpg' width="600">

Pica40 family - ChocV2 with low profile keycaps, ChocV2 with MT3 keycaps, Pica40 v1 with MT3 keycaps, regular switches and hotswap sockets

## Firmware

- QMK - [Source code](https://github.com/zzeneg/qmk_firmware/tree/feature/pica40/keyboards/pica40), [compiled](firmware/qmk/pica40_rev2.uf2)
- ZMK - [Source code](https://github.com/zzeneg/zmk-config), [compiled left](firmware/zmk/pica40_left.uf2), [compiled right](firmware/zmk/pica40_right.uf2), [reset](firmware/zmk/settings_reset.uf2)

## Gerber files

- PCB - [Full](gerbers/full.zip), [Left](gerbers/pcb-left.zip), [Right](gerbers/pcb-right.zip)
- [Bottom plate](gerbers/bottom.zip)
- [Top plate](gerbers/bottom.zip) (not needed for soldered switches)
- [Cover with hole](gerbers/cover-hole.zip) - PCB cover over MCU and rotary encoder (recommended for wireless version)

## Case files (DXF - for metal/acrylic plates)

- [Bottom](dxf/bottom.dxf), [Bottom with tenting holes](dxf/bottom-tenting.dxf)
- [Top](dxf/top.dxf)
- [Cover](dxf/cover.dxf) - cover over MCU and rotary encoder space (for a half without an encoder), [cover with hole](dxf/cover-hole.dxf) - over MCU and rotary encoder (for a half with an encoder). Dark semi-transparent acrylic is recommended for those.

## Bill of materials

- PCBs
- bottom plates
- covers if needed
- 2 XIAO MCUs - [RP2040](https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html) for wired version, [nRF52840](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) for wireless
- 40 SMD SOD-123 1N4148 diodes
- 1 or 2 EC11/12 rotary encoder with knob
- _[Hotswap version]_ top plates
- _[Hotswap version]_ 40 hotswap sockets
- _[Hotswap version]_ 7mm M2 standoffs, 5mm M2 screws
- _[Soldered version]_ 6mm M2 screws, M2 nuts and washers
- _[Wired only]_ [2x USB-C 16pin connector](https://www.aliexpress.com/item/1005003670899595.html)
- _[Wireless only]_ [2x on/off toggle MSK-12C02](https://www.aliexpress.com/item/4000685483225.html)
- _[Wireless only]_ 2x Li-Ion 3.7V battery
- _[Optional]_ sockets and pins for socketing MCUs

## Build log
