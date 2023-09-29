## DAHEIM LADEN SOLAREDGE MODBUS TCP

Home assistant Custom Component for reading data from Daheim Laden wallbox through modbus TCP. Implements wallbox register definitions from https://www.daheimladen.de/_files/ugd/79aefd_1aa1b9522b83486781ef64c67ca7eb62.pdf.

### Features

- Installation through Config Flow UI.
- Separate sensor per register
- Auto applies scaling factor
- Configurable polling interval
- All modbus registers are read within 1 read cycle for data consistency between sensors.
- Supports reading inverter data and meter (1->3) data.
- Supports reading battery data (1->2)
- Supports controlling storedge: Change battery charge / discharge profile

### Configuration
Go to the integrations page in your configuration and click on new integration -> SolarEdge Modbus

<img style="border: 5px solid #767676;border-radius: 10px;max-width: 350px;width: 100%;box-sizing: border-box;" src="https://github.com/binsentsu/home-assistant-solaredge-modbus/blob/master/demo.png?raw=true" alt="Demo">
