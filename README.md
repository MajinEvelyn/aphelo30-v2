# aphelo30
a
![mag usb adapter](https://github.com/MajinEvelyn/aphelo30-v2/blob/main/img/DSCF4149.JPG)
![usb connected](https://github.com/MajinEvelyn/aphelo30-v2/blob/main/img/P6260229.JPG)

Pictured with KLP Lame keycaps that I dyed with [Rit Synthetic Dye](https://www.ritdye.com/type/dyemore-for-synthetics/) using [this method](https://blog.zsa.io/how-to-dye-keycaps/). Case printed in Dark Red PLA.

## Design Parameters
- Full split
- ZMK powered BLE wireless
- Nice! Nano v2 controlled
- Reversible PCB
- 30 keys in 3x5 configuration
- Choc v1 Switches with hotswap sockets
- No thumb keys
- Middle, ring, and pinky splay

Named for the *Aphelocoma* genus of scrub jay birds, like the original. 

## Overview

This weird combination of features is designed for my hands, which no currently existing boards accommodate. I have RSI issues in both of my thumbs, to the point that even single thumb key layouts don't work for me. Aside from this, the aggressive splay and finger positions were made with Ergopad, and recreated in Ergogen. 

Compared to the first version of this keyboard, I adjusted the splay, overall key position, power and reset button positions, and adjusted the PCB and case to accomodate magnetic USB connectors, which I find very convenient. Additionally, instead of a carrying case using a sliding design, this project uses a much more compact magnetic cover to sandwich between both halves.

In this repo you will find all files related to the design process, including the Ergogen config, KiCAD PCB files, related Gerbers, and case 3d files for printing. Unfortunately, I was only able to get the PCB to a 115x85mm footprint with this splay, so a little outside of the <100x100mm discount size for JLCPCB. Despite this and the expensive microcontroller, you should be able to build this board for somewhere between 80-120$.

## Case

There are 4 bosses for heat set inserts on the underside of each half's top case. Press them into each boss with a soldering iron, and use your M2 screws through the holes in the bottom case to screw into the heat set inserts.
There are heat set insert soldering tips available for pretty cheap to make this process easy, but I've heard this is easy enough with typical soldering iron tips.

This case, and PCB is designed with the magnetic USB adapters linked in the BOM, and they sit very flush with the side once assembled. I doubt that other connectors would sit flush in the same way without adjustments to the case design.

The magnets are secured in the cutouts using adhesive, in my case I used B-7000 Clear glue.

![mag usb adapter](https://github.com/MajinEvelyn/aphelo30-v2/blob/main/img/P6260240.JPG)
![usb connected](https://github.com/MajinEvelyn/aphelo30-v2/blob/main/img/P6260242.JPG)

## Carrying Case

This "case" is more of a magnetically attached sandwich cover for the keycaps, and with this arrangement of magnets is very strong. I easily slide into a slot in my camera bag for work.

![carry case](https://github.com/MajinEvelyn/aphelo30-v2/blob/main/img/DSCF4166.JPG)

## Firmware
ZMK: https://github.com/MajinEvelyn/zmk-config-aphelo30
This is the same firmware as the first version, it is fully compatible with both with no changes.

## BOM

| Name | Count | Notes |
| ---- | ----- | ---------- |
| PCB | 2 | These are reversible, so either PCB works with either half. |
| Nice! Nano v2 MCU | 2 | |
| Choc v1 Switches | 30 | |
| Choc v1 Hotswap Sockets | 30 | |
| Choc v1 Keycaps | 30 | |
| Power Switch | 2 | |
| Reset Switch | 2 | You can omit these if you are fine with using ZMK reset behavior or shorting RST pins to reflash firmware. |
| 110mah LiPo Battery | 2 | There is plenty of space for other batteries inside the case, but these can sit underneath the nice! nano. |
| Bumpons | 12 | Size is up to your preference. |
| M2(x8mm) Screws | 8 | Countersunk screws are best, they will seat perfectly into the chamfered holes in the bottom case. |
| M2 Heat Set Inserts | 8 | |
| Magnetic USB C adapters | 2 | https://a.co/d/0hXRvKBZ |
| 5 mm x 1 mm Neodynium Magnets | 16 | https://amfmagnets.com/products/neodymium-disc-5-mm-x-1-mm-gold |
