# How to wire the Z Motors

From the **Swap Board** to the **SKR 3 EZ**:

## Wiring the first Z motor (Z0)
- Run a cable from Z0 1A to ZAM 1A
- Run a cable from Z0 1B to ZAM 1B
- Run a cable from Z0 2A to ZAM 2A
- Run a cable from Z0 2B to ZAM 2B

### Wiring the second Z motor (Z1)
- **Yes, the _E1M_ port is correct.** You are using the second (unused) extruder port as a 5th Z stepper driver. Using _ZBM_ just uses 1 driver for both Z ports, so Z_TILT will not function.
- Run a cable from Z1 1A to E1M 1A
- Run a cable from Z1 1B to E1M 1B
- Run a cable from Z1 2A to E1M 2A
- Run a cable from Z1 2B to E1M 2B

![image](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/assets/139072083/14af0b97-c375-4c78-b4f5-df8d592d491f)

#### If you are using Klipper and the provided firmware, wiring in this manner will both support AND enable "Z_TILT".
- Loosen the bearing retainers at the top of the frame
- Loosen the Z sync belt couplers at the top
- Gently pop off the belt and reasssemble the top side. We leave the GT2 cogs in place.
-- the printer will now sync the Z motors more accurately and perform additional tramming operations.

##### Some Z motors from Anycubic have a reversed phase. The Swap Board kit accounts for this in order to correct it and standardize all motor cable pinouts across the machine. If however, you find that your motor is moving in the opposite direction, reverse one end of the connector.

[Return to installation header](https://github.com/smartwareio/SWIO-Kobra-Max-Adapter-Kit/blob/main/README.md#wiring-the-swap-board)
