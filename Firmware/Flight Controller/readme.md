# Flight Controller Firmware

At least, two firmware revisions are known to exist for the DF806B Flight Controller Board.

- V0.2 includes code for an unknown Optical Flow sensor, not installed on production drones and thus not functional if loaded on a stock unit.
- V1.2 does not need the Optical Flow sensor, and can be loaded on stock units

# Tools

To dump and update FC FW I'veused the ST DfuSe Demo, available for download at: https://www.st.com/en/development-tools/stsw-stm32080.html
