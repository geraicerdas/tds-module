### Repository Content
* **/firmware** : Arduino example codes (.ino)
* **/hardware** : Schematic files (.pdf) some of older version included Eagle design files (.sch and .brd)
* **/production** : gerber file for pcb manufacturing

You can purchase this product from [![Generic badge](https://img.shields.io/badge/Indonesia-Tokopedia-<COLOR>.svg)](https://www.tokopedia.com/geraicerdas/analog-tds-module-for-arduino-water-quality-sensor-tds-module-only) 
[![Generic badge](https://img.shields.io/badge/Worldwide-Tindie-red.svg)](https://www.geraicerdas.com)

# TDS Module

TDS (Total Dissolved Solids) indicates how many milligrams of soluble solids are dissolved in one liter of water. In general, the higher the TDS value, the more soluble solids are dissolved in water. This module can be used in DIY water quality application, such as domestic water analysis and hydroponics. The latest version already have temperature compensation for better accuracy.

<p float="left">
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/3/19/71432b5f-1095-4c65-adab-21ec9e6e0426.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/3/19/a574b25a-a13d-400e-a9ed-2cfe86a32729.jpg" width=400 />
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/3/19/0f2d08f5-2c59-4dc0-804a-7c7bc95fa3ff.jpg" width=805 /> 
</p>

## How To Use
For the hardware you will need :
- Arduino or other compatible microcontroller
- TDS module with TDS probe and waterproof DS18B20
- Jumper wires

(optional : if you want to use Arduino Library) In the Arduino IDE, make sure :
- you have installed Library : [GravityTDS](https://github.com/DFRobot/GravityTDS) by DFRobot (This library tested on Arduino UNO, and will not work with Arduino Leonardo, ESP32)

Connect the TDS module to the MCU
| Arduino / Other MCU | TDS Module |
| ------------- |:-------------|
| 5V / 3.3V | VCC |
| Analog Input Pin | TDS |
| Digital Input Pin | TEM |
| GND | GND |

Upload the code in the firmware folder, and you will get the temperature and compensated TDS value of the water on the Serial Monitor

## Notice
- The probe can not to be used in water above 55 degrees centigrade.
- The probe can not be too close to the edge of the container, otherwise it will affect the reading

## Development logs
V3.0
- Add 3P PH2.0 connector for waterproof temperature sensor DS18B20
- Change 3P terminal to 4P terminal for additional temperature output pin

V2.1
- Rearrange component placement for better layout, fixing wrong decoupling capacitor position
- Change PCB color

V2.0
- Change PCB shape

V1.0
- Initial design

## PCB and Parts

If you want to make your self, just download the gerber file in production folder. Send it to your fav pcb manufacturer. And dont forget to get the Bill of materials :
|Qty | Part Name | Parts | MPN |
| ------------- |:-------------|:-------------| -----:|
|9|Capacitor 0603 100nF|C1, C2, C6, C7, C9, C11, C13, C16, C18|
|3|Capacitor 0603 10uF|C8, C10, C12|
|1|Capacitor 0603 1nF|C15|
|2|Capacitor 0603 1uF|C14, C17|
|2|Capacitor 0603 4.7uF|C4, C5|
|1|Capacitor 3216 100uF|C3|
|2|Resistor 0603 100K-1%|R4, R10|
|7|Resistor 0603 10K-1%|R5, R6, R7, R8, R9, R11, R12|
|1|Resistor 0603 1M-1%|R1|
|1|Resistor 0603 4K7-1%|R14|
|1|Resistor 0603 5.6K-1%|R2, R13|
|1|Resistor 0603 6.8K-1%|R3|
|5|Diode SOD-323 1N4148|D1, D2, D3, D4, D5|
|1|SMD LED 0805|L1|
|1|LMV324 SO-14|U1|
|1|TPS60400 SOT-23-5|U2|
|1|CD4060-BM SO-16|U3|
|1|XC6206P302MR SOT-23|U4|
|1|XH2.5 2P SMD connector|J3|
|1|PH2.0 3P SMD connector|J5|
|1|Teminal Connector 4P 5.08|J6|

Below is the previous version of our TDS Module. We keep this for your references.

### Version 2.1

<p float="left">
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/312c4993-9451-4e73-9aea-a0a2af02289b.jpg" width=268 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/d86db4d8-47f6-4d38-8214-927a6333ce38.jpg" width=268 />
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/37d12968-f82c-4aa1-b497-fbf9aa59bcae.jpg" width=268 /> 
</p>

### Version 1.0

<p float="left">
<img src="images/P1370415.JPG" width=268>
<img src="images/P1370436.JPG" width=268>
<img src="images/P1370463.JPG" width=268>
</p>

## License
*We invests time and resources providing this open-source hardware, please support us by purchasing our products.*

*Designed by **[Insan Sains](https://www.youtube.com/insansains)** for **[Gerai Cerdas](https://geraicerdas.com)**, with contributions from the open source community. Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional information.*
