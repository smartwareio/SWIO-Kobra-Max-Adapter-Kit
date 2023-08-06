# How to wire the Logic Level Shifter and factory print head

From the **BOB 12009** to the **SKR 3 EZ**:
- Run a wire from HV to Z-Stop +5V. _This supplies a 5V reference to the shifter chip._
- Run a wire from GND to GND. _(jump the two grounds together)_
- Run a wire from GND to Z-Stop GND. _This allows the shifter to reference mainboard ground._
- Run a wire from LV to Z-Stop PC0. _This pin is set to 3.3V in the SWIO Config File and allows the shifter to supply 3.3V when 5V from the strain gauge is sent out._
- Run a wire from LV1 to PROBE PC13.
- **You will skip using the PROBE GND connection on the SKR. The shifter is providing ground reference.**

From the **BOB 12009** to the **Swap Board**:
- Run a wire from HV1 to PRB

From the **Swap Board** to the **SKR 3 EZ**:
- Run a wire from PRBRST to SERVO PE5. _This is the pin that resets the strain gauge._
- Run a wire from 5V to SERVO +5V. _This is the pin that powers the toolhead components._
- Run a wire from GND to SERVO GND. _This is the ground reference for the toolhead._
- Run a wire from LED to RGB PE6. _You will not use the other pins on RGB._

![image](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/assets/139072083/d990462d-854e-40e7-b60e-4a5a26f215d4)

[Return to installation header](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/installation/shifter_printhead.md)
