### Repository Content
* **/firmware** : Arduino example codes (.ino)
* **/hardware** : Schematic files (.pdf) some of older version included Eagle design files (.sch and .brd)
* **/production** : gerber file for pcb manufacturing

You can purchase this product from [![Generic badge](https://img.shields.io/badge/Indonesia-Tokopedia-<COLOR>.svg)](https://www.tokopedia.com/geraicerdas/analog-tds-module-for-arduino-water-quality-sensor-tds-module-only) 
[![Generic badge](https://img.shields.io/badge/Worldwide-Tindie-red.svg)](https://www.geraicerdas.com)

# TDS Module

Since the schematic design is based on DFRobot product :
https://www.dfrobot.com/product-1662.html so the library and sample codes can refer to their documentation :
https://wiki.dfrobot.com/Gravity__Analog_TDS_Sensor___Meter_For_Arduino_SKU__SEN0244

## How To Use
For the hardware you will need :
- Arduino or other compatible microcontroller
- TDS module with TDS probe
- Jumper wires

(optional : if you want to use Arduino Library) In the Arduino IDE, make sure :
- you have installed Library : [GravityTDS](https://github.com/DFRobot/GravityTDS) by DFRobot

Connect the TDS module to the MCU
| Arduino / Other MCU | TDS Module |
| ------------- |:-------------|
| 5V / 3.3V | VCC |
| Analog Input Pin | OUT |
| GND | GND |

Upload the code in the examples, and you will get the TDS value of the water on the Serial Monitor

## Notice
- The probe can not to be used in water above 55 degrees centigrade.
- The probe can not be too close to the edge of the container, otherwise it will affect the reading

## PCB and Parts

<p float="left">
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/312c4993-9451-4e73-9aea-a0a2af02289b.jpg" width=400 /> 
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/d86db4d8-47f6-4d38-8214-927a6333ce38.jpg" width=400 />
<img src="https://images.tokopedia.net/img/cache/900/VqbcmM/2022/1/21/37d12968-f82c-4aa1-b497-fbf9aa59bcae.jpg" width=805 /> 
</p>

If you want to make your self, just download the gerber file in production folder. Send it to your fav pcb manufacturer. And dont forget to get the Bill of materials :
|Qty | Part Name | Parts | MPN |
| ------------- |:-------------|:-------------| -----:|


Below is the previous version of our TDS Module. We keep this for your references.

### Version 1.0

<p float="left">
<img src="images/P1370415.JPG" width=268>
<img src="images/P1370436.JPG" width=268>
<img src="images/P1370463.JPG" width=268>
</p>

## License
*We invests time and resources providing this open-source hardware, please support us by purchasing our products.*

*Designed by **[Insan Sains](https://www.youtube.com/insansains)** for **[Gerai Cerdas](https://geraicerdas.com)**, with contributions from the open source community. Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional information.*
