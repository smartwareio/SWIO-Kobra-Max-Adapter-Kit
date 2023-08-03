# This is a current repo of the Smartware/IO PCB adapter to convert the Anycubic Trigorilla Pro A104/B102 boards to JST connectors, so that the factory harness can be reused.
## You will need:

- A pair of JST crimpers
- A set of JST-XH connectors and pins
- Some 20-22ga stranded wire. Ribbon cable that comes with Dupont kits is hit or miss here. For the heater jumper, we recommend that you use 20-22AWG silicone (high heat) wire.

Start by selecting a board. **We recommend using the BTT SKR 3 EZ.** The pinout and wiring diagrams will be provided here.

Be sure to match GND to GND on your board for every connection. The Smartware boards are marked, but not all printer boards are. You will need to refer to the _pin schedule_ for your particular board to ensure that this is correct. **Getting these wrong or reversed will result in errors and improper machine operation.**

Anycubic has reversed the stepper phase on the X motor for some Max printers. We have corrected for this in the adapter board, but your milage may vary here. If your X stepper moves in the wrong direction, you will need to reverse one connector end for your motor.

### If you are using the factory strain gauge and omitting the Extruder Board:

- Install a logic level shifter such as the Sparkfun BOB.
- Set a spare pin of your board to 3.3V out constant
- Wire the 3.3V to the LV pin on the BOB12009
- Wire a 5V mainboard pin to the HV pin on the BOB12009
- Jump GND together on both sides of the BOB12009, then run that to a GND pin on your mainboard
- Wire the PRB coming from the adapter board to HV1
- Wire the LV1 to the probe pin to your motherboard
- **Most shifters do not have mounting provisions as they are tiny. You can hot glue it or modify the board adapter plate to have some tabs for it if you wish.**
- **The level shifter is REQUIRED to be used with the factory print head. The factory head sends 5V out into the GPIO upon reset. The shifter brings this to safe levels.**
