CAN-Bus_Shield_v1.2
====================

I updated the schematic to migrate the SPI connections over to the ICSP header to allow the Shield to be compatible with other Arduinos that do not use digital pins 11-13 for SPI.  I also provided the option to select /INT pin.

This version is capable of operating at 3.3V BUT the MCP2562 still needs +5V to operate the CAN bus.  There is a solder-jumper pad to select the voltage of operation if IOREF pin is not used.

This version has two pinouts on the DE9 for CAN.  These two pinouts are not enabled by default, there are three solder-jumpers on the bottom of the PCB.  The dots indicate the "Standard CAN Pinout" commonly used and the opposite retains compatibility with the OBDII cable which started this whole mess.

This version features a split termination that is not enabled by default.  The split termination improves CMRR.
