
# Compile Settings
1) Go to https://kno.wled.ge/advanced/compiling-wled/ and follow the steps needed to create your own binary.
2) Once done, rename your plaformio.ini to plaformio_BCK.ini in your WLED Folder.
3) Download CompileSettings/Platformio_RGBFighter.ini and paste it in your WLED Folder
4) Recompile for from this repositoryand open in your IDE Environement (Platformio compatible).
Rename your current Pl

# First-Use


# Components
- Temperature Sensor : DS18B20
- Level Shifter : 74HCT245DW with 200Ohm resistance on each output
- USB-C PD Trigger : IP2721 with fixed voltage

# Voltage Input
Voltage Divider for Power Monitoring. Ships fixed in the choosen USB-C Trigger.

Vin	| R2 Ohms	| R3 Ohms
--- | --- | ---
20V |	1000	| 170
12V	| 1000	| 300
5V	| 1000	| 1200

# Pinout
Pin | Description | Pin | Description
--- | --- | --- | ---
LED D1 | IO14 | LED D2 | IO15
LED D3 | IO17 | LED D4 | IO13
Voltage | IO35 | Temperature | IO02

# Warranty & Risk
