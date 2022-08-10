# Pica40

Split keyboard with 40 keys and 1 ProMicro-compatible controller.

_Pica pica - european (common) magpie_

<img src='images\full.jpg' width="600">

## Features

- 40 MX keys with Kailh hotswap sockets
- single ProMicro-compatible controller
- hotwired cable between halves (or custom USB-C cable)
- rotary encoder on second side (without click)
- on/off toggle and battery connector for wireless compatibility
- OLED display
- aggressive stagger
- one status LED

<img src='images\led.jpg' width="600">

## Renders

Left (MCU) side

<img src='images\render-pcb-left-front.png' width="600">
<img src='images\render-pcb-left-back.png' width="600">

Right side

<img src='images\render-pcb-right-front.png' width="600">
<img src='images\render-pcb-right-back.png' width="600">

## Bill of materials

Gerbers - to be printed by manufacturer (all files have jlcpcb marks, remove if using something else):

- PCB - [left](gerbers/pcb-left.zip) and [right](gerbers/pcb-right.zip)
- Top plate - [top](gerbers/top.zip) is reversible, can use 2 for both halves or 1 + [right](gerbers/pcb-right.zip) doesn't require a separate cover (not tested). [left](gerbers/top-left.zip) is same as _top_ but for aluminum plate.
- [Bottom plate](gerbers/bottom.zip) x2
- [Cover](gerbers/cover.zip) x2 (can be replaced with acrylic if wanted)

Alternative plates (not tested):

- [metal/acrylic bottom](dxf/bottom.dxf)
- [metal bottom with tenting holes](dxf/bottom-tenting.dxf)
- [acrylic cover](dxf/cover-acrylic.dxf)
- metal top plates - [left](dxf/plate-metal-left.dxf) and [right](dxf/plate-metal-right.dxf)

Electronics:

- Arduino Pro Micro or compatible
- 40 hotswap sockets
- 40 SMD SOD-123 1N4148 diodes
- cable with 12 wires, optionally cable sleeve and heat shrink tube
- m2 screws, nuts and 8mm standoffs
- EC11/12 rotary encoder with knob
- 2 reset buttons

## Build log

I was not able to solder a custom USB-C cable as I wanted initially so I had to hotwire a cable. Still works though.

<img src='images\back.jpg' width="600">
<img src='images\back-1.jpg' width="600">
<img src='images\back-2.jpg' width="600">

## Firmware

[QMK with Vial support](firmware/pica40_vial.hex)
