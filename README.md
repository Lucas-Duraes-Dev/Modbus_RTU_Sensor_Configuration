# Modbus_RTU_Sensor_Configuration
Python script for configuring Modbus RTU sensors.

This script assumes that a dictionary with the following parameters are given:

- **FMA[Mandatory]**  Factory Modbus address of the sensor
- **RMA[Mandatory]**  Register which contains the sensor Modbus address
- **RBR[Mandatory]**  Register which contains the baud rate information of the sensor
- **CRMA[Optional]**  Desired Modbus address for the sensor; the script will change the FMA address to the CRMA address
- **CRBD[Optional]**  Desired Modbus baudrate for the sensor; the script will change the current baudrate to the CRBD baudrate
- **CRX**: Custom commands, like reading or writing to certain registers. Will execute in order(so for example, CR1, then CR2, then CR3, and so forth)

Check **example.py** for more information on how to create this dictionary data structure.
