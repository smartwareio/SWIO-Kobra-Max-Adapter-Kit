# Welcome to the documentation for the SWIO Kobra Max Swap Kit. Here you will find information required to utilize the _Swap Board_ and _Extruder Board_ in the kit. Please note that this kit is currently in BETA and is a _work in progress_.

**Found this page without knowing about the product? Get it [here](https://www.smartwareio.com/product/kobra-max-mainboard-and-print-head-kit/9)!**

## You will need:

- To purchase or print a set of adapter plates [See the STL section](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/tree/main/STL) **If you are self-printing adapters, you will also need heat-sets, which are linked**
- A pair of JST crimpers
- A set of JST-XH connectors and pins
- Some 20-22ga stranded wire. Ribbon cable that comes with Dupont kits is hit or miss here. For the heater jumper, we recommend that you use 20-22AWG silicone (high heat) wire.
- _Optional, but recommended_: A ferrule crimper and ferrules for shortening or attaching multiple conductors together. You will likely need these for the cables on the NF103 bed heater board.

[**Recommended crimper and JST kit here** (Amazon)](https://amzn.to/3KvIH76)

[**Recommended cable for 2-wire connections here** (Amazon)](https://amzn.to/3Qx5LGw)

[**Recommended cable for 4-wire connections here** (Amazon)](https://amzn.to/3OPArBC)

[**Ferrule and crimper kit**](https://amzn.to/3qjfENh)

Start by selecting a board. **We recommend using the BTT SKR 3 EZ.** The pinout and wiring diagrams will be provided here.

Be sure to match GND to GND on your board for every connection. The Smartware boards are marked, but not all printer boards are. You will need to refer to the [_pin schedule_](https://github.com/bigtreetech/SKR-3/blob/master/Hardware%20(SKR%203%20EZ)/BIGTREETECH%20SKR%203%20EZ%20V1.0-PIN.pdf) for your particular board to ensure that this is correct. **Getting these wrong or reversed will result in errors and improper machine operation.**

Anycubic has reversed the stepper phase on the some motors for some Max printers. We have corrected for this in the adapter board, but your milage may vary here. If your stepper moves in the wrong direction, you will need to reverse one connector end for your motor. Our boards account for the Max we have available for development and have made all cables "striaght-through" style.

**The factory display is not going to work with this kit directly. There are mods that can be done, but we do not support them.**

### If you are using the factory strain gauge and omitting the Extruder Board:

- Install a logic level shifter such as the [Sparkfun BOB](https://amzn.to/3QuQJ40).
- See [Wiring the Swap Board](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/tree/main#wiring-the-swap-board) for instructions on how to use it.
- **Most shifters do not have mounting provisions as they are tiny. You can hot glue it or modify the board adapter plate to have some tabs for it if you wish.**
- **The level shifter is REQUIRED to be used with the factory print head. The factory head sends 5V out into the GPIO upon reset. The shifter brings this to safe levels.**

#### Wiring the Swap Board

- [FAN0 / FAN1](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/fans.md)
- [Heater (extruder)](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/heater.md)
- [Thermistor (extruder)](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/thermistor.md)
- [Z Optical](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/z_optical.md) (you may skip this if using Klipper)
- [Filament Runout Sensor](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/runout.md)
- [X Stop](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/xstop.md)
- [Y Stop](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/ystop.md)
- [E Motor](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/emotor.md)
- [X Motor](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/xmotor.md)
- [Y Motor](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/ymotor.md)
- [Z0 Motor, Z1 Motor](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/zmotors.md) (and special note)
- Factory Kobra Max connections
- [Factory strain gauge/toolhead & required Logic Level Shifter](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/shifter_printhead.md)
- Factory NF103 Heater Board

  ##### Printer Profiles

  - Check out the [Cura Project Files](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/tree/main/CuraProjectProfiles) folder for some premade profiles that we have been using and fine tuning for several months.
