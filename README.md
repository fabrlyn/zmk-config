# zmk-config

Configuration for my Aurora Corne.

![keyboard](https://drive.google.com/uc?id=1d2KR6ojLhsbK5TKA0mCipWTqPQBE-k3F)

## setup

- Clone this repository
- Setup zmk [toolchain](https://zmk.dev/docs/development/setup)

## building and flashing

- Make the `/<ABSOLUTE-PATH>/zmk/app` path the current working directory.
- Replace placeholder path and run: `west build -b nice_nano_v2 -- -DSHIELD=splitkb_aurora_corne_left -DZMK_CONFIG="/<ABSOLUTE-PATH>/zmk-config/config"`.
- Connect the left half and double click the reset button.
- Drag the `/<ABSOLUTE-PATH>/zmk/app/zmk.uf2` to the root directory of the `NICENANO` usb device.
- Disconnect the left half, done!

## bill of materials

### case

- AUR-CRN-ABB-002 Aurora Corne Low Profile Case Bottom Plate / Black Acrylic / Set of 2 1
- AUR-CRN-FTB-002 Aurora Corne Low Profile Case Top Plate / Black FR4 / Set of 2 1
- AUR-HWK-LOW-001 Aurora Low Profile Case Hardware Kit 1

### electronics

- AUR-CRN-BHK-010 Aurora Corne PCB Kit Choc/MX Hand solder 1
- CMP-N2N-UPG-JSW Wireless Controller Expansion Bundle / 1
- MMX-LPS-0SK-P25 Mill Max Low Profile Sockets 25 Pins 1
- MMX-LPS-2SK-P25 Mill Max Low Profile Sockets Set of Sockets with Pins 2
- NNT-N1N-020-001 nice!nano Wireless Microcontroller 2.0 / 2
- LiPo 3.7V 130mAh / 2

### keycaps

- KSM-MBK-CBL-010 Coloured Blank MBK Choc Low Profile Keycaps Blue (2728U) / 10 keycaps 1
- KSM-MBK-COR-010 Coloured Blank MBK Choc Low Profile Keycaps Orange (1665U) / 10 keycaps 2
- KSM-MBK-CPB-001 Coloured Blank MBK Choc Low Profile Keycaps Pastel Blue (0821U) / 1 keycap 5
- KSM-MBK-CPY-001 Coloured Blank MBK Choc Low Profile Keycaps Pastel Yellow (0131U) / 1 keycap 4
- KSM-MBK-CRD-001 Coloured Blank MBK Choc Low Profile Keycaps Red (185U) / 1 keycap 3

### switches

- KLH-CHC-BRN-010 Kailh Low Profile Choc Switches Brown (tactile / 50gf) / 10 switches 5

## assembly notes

### top plate

The battery switch height interferes with the top plate, there isn't enought room height-wise.

The solution was to saw and file of the edge of the top plate, this did the trick.

### battery

The battery did not fit between the bottom plate and the pcb. Glueing the battery on to the top of the controller worked fine. 

Since the controller is mounted upside down the surface is component free and smooth.
