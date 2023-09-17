klipper
v0.11.0-271-g5f990f93

Compiled for STM32H723 which is NOT the advertised CPU that the SKR 3 EZ comes with. Some 3 EZ boards are shipping with this CPU. This firmware is set for USB connection. If you need serial connection or CAN, you will need to use the make menuconfig and recompile.

Put the firmware.bin onto a BLANK SD card, 16GB or less. Do a quick format FAT32, copy the firmware.bin to the card. Eject the card and remove from your machine. Turn OFF your printer, insert the card, turn on the printer. Count to 5, turn the printer off and remove the card.

To confirm the firmware loaded, insert the SD back into your computer. The "firmware.bin" file should be renamed "FIRMWARE.CUR".
