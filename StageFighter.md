
# Compile Settings
1) Go to https://kno.wled.ge/advanced/compiling-wled/ and follow the steps needed to create your own binary.
2) Once done, rename your plaformio.ini to plaformio_BCK.ini in your WLED Folder.
3) Download CompileSettings/Platformio_RGBFighter.ini and paste it in your WLED Folder
4) Recompile for from this repositoryand open in your IDE Environement (Platformio compatible).
Rename your current Pl

# First-Use
1) Connect your leds to your setup
The most typical setup is to use 12V 
2) 
3) Connect your Power Supply
- USB-C (Check the label rating on your power supply if it can deliver the requested voltage
- DC Barrel with Pin Positive 2,1 mm
- Screw Terminal Adaptor
- Solder your own XT30 Connector!

3) df

# Components
- Temperature Sensor : DS18B20 for internal enclosure monitoring
- Level Shifter : 74HCT245DW with 200Ohm resistance on each output
- DCDC Converter : ME3116 (max Voltage 40V)
- USB-C PD Trigger : IP2721 with fixed voltage set (max Voltage 30V)

# Pinout
Pin | Description | Pin | Description
--- | --- | --- | ---
LED D1 | IO14 | LED D2 | IO15
LED D3 | IO17 | LED D4 | IO13
Voltage | IO35 | Temperature | IO02

# Voltage Input
Voltage Divider for Power Monitoring. Ships fixed in the choosen USB-C Trigger.

Vin	| R2 Ohms	| R3 Ohms
--- | --- | ---
20V |	1000	| 170
12V	| 1000	| 300
5V	| 1000	| 1200

# Warranty & Risk
Current 20AWG Silicon Wire - Around 5Amp

