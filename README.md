[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/custom-components/hacs)

# home-assistant-daheim-laden-modbus
Home assistant Custom Component for reading and writing data from Daheim Laden wallbox through modbus TCP.
Implements wallbox registers according to the [Daheim Laden API documentation of the Modbus tcpip interface][1]

# Installation
Copy contents of custom_components folder to your home-assistant config/custom_components folder or install through HACS.
After reboot of Home-Assistant, this integration can be configured through the integration setup UI

# Enabling Modbus TCP on Daheim Laden wallbox
1. Ask the daheim laden service to install latest firmware version with ModBus enabled. 
2. Find out the IP and ModBus port (usually 12345) of your wallbox
3. 

# Control of charge settings 
There are 3 states for charging: 
1. IDLE
2. START Charging - Enables the Charging Process. The charging starts only if the vehicle accepts it (e.g. the battery is not yet fully charged or below the defined max state of charge)
3. STOP Charging

The charge current can be set, too. However, there are 2 registers for defeining the max charge current which may interact if not set properly. 
- B
- C

Remark: External charging control software 

[1]: https://www.daheimladen.de/_files/ugd/79aefd_1aa1b9522b83486781ef64c67ca7eb62.pdf 
