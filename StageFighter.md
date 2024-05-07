
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

# Poweer Input
## Voltage Selection
The XT30 allows the user to deliver voltage up to 30V to its strips. Often Pixels like the popular WS2815 relys on 12V.
This power can be sourced by 
By choosing and USB-B 2.0 to USB-C Cable with a USB 2.0 Power Supply, you'll deliver 5V to your led strips. 
However due the integrated DCDC Converter you need to at least a stable 5.0V power source. 

## Current Rating
Current 20AWG Silicon Wire - Around 5Amp
## Voltage Divider for Power Monitoring. Ships fixed in the choosen USB-C Trigger.
Vin	| R2 Ohms	| R3 Ohms
--- | --- | ---
20V |	1000	| 170
12V	| 1000	| 300
5V	| 1000	| 1200

# Disclaimer and Warranty Information

## Use Qualification: 
The RGBFighter is designed for users who are qualified and experienced in electronics. Handling and installation of the device should only be performed by individuals who understand the safety precautions necessary for electronic devices.

## Operating Conditions: 
The RGBFighter is not designed for use in harsh environmental conditions. Do not operate the device outdoors, in wet conditions, or in any situation where it is exposed to moisture or extreme temperatures. The device must be monitored during operation to ensure safety and proper functioning.

## Warranty: 
This product is provided 'as is' without any express or implied warranties. The creators of the RGBFighter are not liable for any damages or injuries resulting from the use or misuse of this product. Use at your own risk.

## Maintenance:
Regular checks and maintenance are recommended to ensure the product's longevity and optimal performance.

