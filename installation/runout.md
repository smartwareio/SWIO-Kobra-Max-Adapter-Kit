# How to wire the filament runout sensor
_Please note that there will be two ways to go about this_. If you are using the factory print head and have only swapped the mainboard, you will only be connecting to the **Swap Board**.
If you are using both the **Swap Board** _and_ the **Extruder Board**, you will need to run a new length of cable directly from the SKR to the top of your frame. This is because the runout sensor in the factory location will no longer work for you, and you have converted to Direct Drive.

## "I am reusing the factory Kobra Max Print head":

From the **Swap Board** to the **SKR 3 EZ**:

- Run a wire from FLMT GND to E0DET GND
- Run a wire from FLMT I/O to E0DET PC2

![image](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/assets/139072083/6156724c-3a32-4a75-83cb-cc78d270d2e3)

### "I am using the Extruder Board for a direct drive conversion":

- Do not wire your sensor to the swap board. Wire it directly to the mainboard ports. As a bonus, you now have 3 wires to use and can have an LED on the sensor (utilize the 5V pin).
- Wire a 3 conductor length of wire and run it up the right frame support to the top of the frame. You will find a printable file to use a standard filament sensor up top.

![image](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/assets/139072083/2d968ce2-d4d3-4454-9d73-b15c3a9eb017)

[Return to installation header](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit#wiring-the-swap-board)
