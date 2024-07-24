# First-Use
1) Connect your leds to your setup
RGBFighter is intented to use with 12V LED Pixel Strips featuring one data pin (no clock) and two (Positive-Negative).
There are two option to connect the board to the strips.
- Screw Terminal : Use a 2mm screwdriver to secure the 3 wires or Cable Guard in the following order (from right to left): + / Data / -
- Preconfected Cable Connector
Take care about polarity. You can use a DMM to double check voltage and continuity.

2) Connect Your Power Supply
Depending on the number of pixels, select a power supply with sufficient capacity. Use the WLED power calculator: https://wled-calculator.github.io
Example: A setup with four 5-meter-long LED strips at 30px/m draws approximately 8 amps at maximum brightness, exceeding device specifications.
Options for power supply connection:
- USB-C Supply or Power Bank
- ACDC Power Supply with a barrel jack (positive pin inside, 2.1 mm)
- Screw Terminal Adaptor to fix the cable of your choice
- Solder your own XT30 Connector (female). Silicon cables are easier to solder as they won’t melt as easily.
  
3) You’re Ready to Go
Follow the standard routine and tutorials from the WLED community. Happy RGBFighting!
Double-check the ratings of your power supply, especially when using USB-C PD to deliver more than 5V. Check the label rating on your power supply to ensure it can deliver the requested voltage.

# Programming & Compile Settings
## Integrate RGBFighter Definitions in your PlatformIO
1) Visit https://kno.wled.ge/advanced/compiling-wled/ and follow the steps to create your own binary.
2) Once done, rename your platformio.ini to platformio_BCK.ini in your WLED folder.
3) Download CompileSettings/Platformio_RGBFighter.ini and paste it into your WLED folder.
4) Recompile from this repository and open in your IDE Environment (PlatformIO compatible).
5) Follow the normal OTA procedure for upload.

## Physical progamming
1) Disassemble your StageFighter and remove the front plate and all wires attached to it.
2) Remove the shield with the level shifter and place the Flash Device.
<img width="400" align="center" alt="image" src="https://github.com/alfredtorch/RGBFighter/assets/38537119/994f9a3d-ce73-43d7-885c-54849e86dcc2">

Flash device is not yet available on Tindie.

# Power Input
## Voltage Selection
The XT30 connector allows you to deliver up to 30V to your strips. WS2815 pixels, for example, rely on 12V.
By using a USB-B 2.0 to USB-C cable with a regular USB 2.0 power supply, you'll deliver 5V to your LED strips (backward compatibility).
However, due to the integrated DC-DC Converter, you need to ensure a stable 5.0V power source. Measure this with an inline USB power tester.

## Current Rating
Current 20AWG Silicon Wire - Around 5Amp
## Voltage Divider for Power Monitoring. Ships fixed in the choosen USB-C Trigger.
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

# Screenshots
<p align="center">
<img width="414" alt="image" src="https://github.com/user-attachments/assets/ea154ab8-46f6-4474-91d6-c6d62deef15a">
<br>
<img width="412" alt="image" src="https://github.com/user-attachments/assets/9bfa872e-36bf-4cfb-9213-eee87ca6a54c">
<br>
<img width="412" alt="image" src="https://github.com/user-attachments/assets/b0d17ddc-19ed-4621-91e2-c626a665fda6">
</p>

# Components
- Temperature Sensor : DS18B20 for internal enclosure monitoring
- Level Shifter : 74HCT245DW with 200Ohm resistance on each output
- DCDC Converter : ME3116 (max Voltage 40V)
- USB-C PD Trigger : IP2721 with fixed voltage set (max Voltage 30V)

# Version & Development Roadmap
Design Issues: None reported
Etended Temperature Usage: Success (needs to be documented).
Heavy Duty Testing: Maximum Current Setting & Long-term in production field needs to be completed.
<img src="https://github.com/alfredtorch/RGBFighter/assets/38537119/d63631b6-a65c-419a-85b1-2c38ca4941f8)" align="center" width="800px">

# Disclaimer and Warranty Information

## Use Qualification: 
The RGBFighter is designed for users who are qualified and experienced in electronics. Handling and installation of the device should only be performed by individuals who understand the safety precautions necessary for electronic devices.

## Operating Conditions: 
The RGBFighter is not designed for use in harsh environmental conditions. Do not operate the device outdoors, in wet conditions, or in any situation where it is exposed to moisture or extreme temperatures. The device must be monitored during operation to ensure safety and proper functioning.

## Warranty: 
This product is provided 'as is' without any express or implied warranties. Should you encounter any problems, we strongly encourage you to contact us directly to assess the situation. Note that this support does not cover damages attributable to improper installation, connection to incorrect voltages, abuse, alteration, or misuse. The components are part of a broader assembly that is the responsibility of the user to complete and operate correctly. The creators of the RGBFighter are not liable for any damages or injuries resulting from the use or misuse of this product. Use at your own risk.

## Maintenance:
Regular checks (e.g., broken wires, enclosure damage) are recommended to ensure the product's longevity and optimal performance.
