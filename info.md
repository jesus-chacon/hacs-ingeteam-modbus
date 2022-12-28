## INGETEAM solar inverter for Home Assistant

Home assistant Custom Component for reading data from Ingeteam inverter through modbus TCP. Implements Inverter registers from https://www.ingeconsuntraining.info/?page_id=25439.

This custom component is experimental version with featured not (yet) present in standard Hass integration and is

### Features

- Installation through Config Flow UI.
- Separate sensor per register
- Configurable polling interval
- All modbus registers are read within 1 read cycle for data consistency between sensors.
- Possible to select other modbus address than the default of 1
- Supports reading inverter data
- Supports reading external meter data
- Supports reading battery data
- Create cumulative energy values from de instant measurements with Riemann Sum integration.
- Added total imported/exported/PV powers as absolute sensors.
- Added charge and discharge power sensor for battery

### Configuration

Go to the integrations page in your configuration and click on new integration -> Ingeteam Modbus
