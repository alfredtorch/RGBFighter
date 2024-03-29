<img src="images/Banner.jpg?raw=true">

🚥 Micro ESP-01 board for addressable pixel control 🚥 ... suits to every place and mostly to any needs!
Only a power bank and a smartphone are needed and you're good to go with your mobile setup.

* Small : +- 14x32mm & Lightweight : +- 4gr
* ESP8266 based (Support for Arduino)
* Designed for common LED Strips like WS2812 with level shifting
* Connection over 2,54 mm 3 Pin for direct soldering, JST or screw terminal (Version Strip or Panel)
* Power and Progamming over USB (CP2104 nodeMCU design)
* User Input for One Button OR IR Receiver
* [WLED](https://github.com/Aircoookie/WLED "WLED's Github page") compatible
* Inspirations from Adafruit, Sparkfun and many others


<img src="images/RGBFighterFamily.jpg?raw=true">

# ⚡️PCB 
<img src="images/BottomBoard.jpg?raw=true" align="center">
<img src="images/TopBoard.jpg?raw=true" align="center">


# 🔦 Hardware

At the moment I have no possibility for a larger production and distribution. Of course, I am ready for any cooperation to industrialize the production. Happy to get any proposition.

## 🗺 Design Files

Designed in Eagle, in a messy way! Sorry! The related files are available under /Hardware.
Name | Description 
--- | ---
ButtonPanel | Panel and Button
ButtonStrip | Strip and Button
IR | Strip and IR Receiver
PowerRail | Power for 8 Strips
PowerDistributorX30 | 5 Ports XT-30 Connector

## 🛠 For DIY'er:
All you need are steady hands for the soldering part, specially the QFN. A reflow or hot plate is suggested.
The thickness of the board should be 1,2mm in order to sold the vertical USB firmly. The parts can be easily ordered from the common suppliers.

## 💰BOM

Part Name | Quantity | Price | Supply Link | Notes 
--- | --- | --- | --- | ---
Board RGBFighter | 1 | 0,02€ | [DirtyCheapPCB](https://dirtypcbs.com/store/pcbs/buy/108056/rgborder10x10january2019-zip) | Panelised Design files of Panel-Strip-USB Versions
ESP-01 MCU | 1x | 2€ | [Amazon](https://amzn.to/3qxXip7) | The brain with Wifi!
CP2104 USB Controller | 1x | 3€ | Mouser, ... | need for progamming : alternative [ESP-01 Flasher Amazon](https://amzn.to/3A2HptF) - [Aliexpress](https://s.click.aliexpress.com/e/_9JcISN)
Micro USB Vertical | 1x | 0,5€ | [Aliexpress](https://s.click.aliexpress.com/e/_AaeVzr)
Resistor Array 603 10k | 2x | 0,2€ | Mouser, ... | Pull-up registors for programming and normal operation
Transistor MMBT2222 | 2x | 0,2€ | Mouser, ... | need for programming, NPN Type
Capacitor 0805 | 3x | 0,2€ | Mouser, ... | Various values : schematics
Inducator 2.2uH | 1x | 0,2€ | Mouser, ... | NRH2412T2R2MNGH
3V3 Step Down Converter | 1x | 1,2€ | Mouser, ... | LM3671
Reistor 300Ohm 0805 | 1x | 0,2€ | Mouser, ... | basic pin protection 
Level Shifter SN74LVC1T45DBV  | 1x | 0,2€ | Mouser, ... | for the right Voltage on the Data bus
Button G71Y | 2x | 0,2€ | [Aliexpress](https://s.click.aliexpress.com/e/_A68Ds9) | MCU & Reset User Input
IR Receiver | 1x | 0,2€ | [Aliexpress](https://s.click.aliexpress.com/e/_A7jhiZ) |IR Control Version

🙏 Please if you need to shop for parts, it would be great that you use the supply links below. As they are affilated, you're supporting me directly to continue to deliver new projects to the community! Thank you ❤️
<p align="center">
<img src="https://user-images.githubusercontent.com/38537119/155808479-0642d7e2-f94d-4171-adef-1f9d71b3f145.png"  width="320">
</p>

# 🎆 Versions
<img src="images/OneButton.jpg?raw=true" align="center">
<img src="images/IrControl.jpg?raw=true" align="center">
<img src="images/MatrixBuddy.jpg?raw=true" align="center">

# 📖 History and Evaluation

It started longtime ago when I wanted an easy way to drive my pixels. First pcb version was sended to fabrication in july 2016. 
Since the project evolved into something more advanced and more mature!

## 🔍 Development Phase
ToDo | Remarks
--- | --- 
Easy Boards | Design boards without programming chip but with easy to solder buttons and voltage converter 
Documentation | Improve the transfer of knowledge
Big production | Looking forward to have some input, help to release it massivly, if wanted.

# 🛒 Accessories

Most of these parts can be laser cutted. The related files are available under Hardware/RGBFighterLaserParts.dxf

<img src="images/StorageBox.jpg?raw=true" align="center">
<img src="images/USBPowerInjector.jpg?raw=true" align="center">
<img src="images/LaserParts.jpg?raw=true" align="center">
<img src="images/8PowerRail.jpg?raw=true" align="center">

# 👶🏼 First Steps & Ideas

⚠️Don't mess with the power - no polarity or whatever protection ⚠️

⚠️Vertical USB is fragile - Handle with care ⚠️

## 🤏🏽 Pinout
Pin | Function
--- | ---
GPIO0 | Button Or InfraRed
GPIO2 | RGB Output | Recomanded Output from WLED

## 💾 Programming
You can directly check the [How-To from WLED](https://kno.wled.ge/basics/install-binary/)

## 🪛 Tutorials
see [Tutorials Page](https://github.com/alfredtorch/RGBFighter/blob/master/Tutorials.md)

<img src="images/8x8Projector.jpg?raw=true" align="center">
<img src="images/PowerBank.jpg?raw=true" align="center">
<img src="images/MagneticStrip.jpg?raw=true" align="center">

Servo, Electro-Dipped, ...

---

# ⚖️ Licence
The MIT License (MIT)

Copyright (c) 2021 Max Schmit

Permission is hereby granted, free of charge, to any person obtaining a copy of this Hardware and associated documentation files (the "Hardware"), to deal in the Hardware without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Hardware, and to permit persons to whom the Hardware is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE HARDWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

<a href="https://trackgit.com">
<img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/l155l9mocavsiw6xftl1" alt="trackgit-views" />
</a>
