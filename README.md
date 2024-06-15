# RCM-Hardware-BYTE
v2.3

* 1.25 by 1.25 inches, 31.75 by 31.75 millimeters
* 8 motors
* 8 servos
* battery monitoring
* I2C connector on QT PY
* runs on 3-11 volts

### Tested with the following types of ESP32 QT Py:
| Type of Qt Py | PlatformIO name | link to Adafruit |
| ------ | -------- | -------- |
| S3 with 2MB PSRAM |  adafruit_qtpy_esp32s3_n4r2   |  https://www.adafruit.com/product/5700   |
| S3 with 8Mb Flash |  adafruit_qtpy_esp32s3_nopsram   |  https://www.adafruit.com/product/5426   |
| S2 |  adafruit_qtpy_esp32s2   |  https://www.adafruit.com/product/5325  |

Look here for how to program it: https://github.com/RCMgames/RCMv2

Look here for more information and examples of robots: https://github.com/rcmgames

Want slightly smaller with a built in IMU? Look at the [Nibble](https://github.com/RCMgames/RCM-Hardware-Nibble)

## Options for purchasing

* [PCBWay link](https://www.pcbway.com/project/shareproject/RCMHardwareByte_v2_3_e23eec63.html) (PCBWay will give me a commission without increasing the price for you). (approximately $90 for 2 boards and manufacturing took a month).
* send the gerbers, bill of materials, and ComponentPlacement files to a PCB manufacturer of your choice (details you may be asked for: min hole 0.25mm, min track/spacing 5/5mil, thickness 1.0mm, 1 oz Cu outer 1.5 oz Cu inner)

## Components
Solder by hand to complete the assembly of your boards.
| part | links | quantity | notes |
| ----- | ----- | ----- | ----- |
| RCM Nibble circuit board | [options for purchasing](https://github.com/RCMgames/RCM-Hardware-BYTE/tree/main#options-for-purchasing) | 1 | |
| ESP32 QT Py | [compatible QT Py](https://github.com/RCMgames/RCM-Hardware-BYTE/tree/main#tested-with-the-following-types-of-esp32-qt-py) | 1 | |
| 2x8 female header pins | [this](https://www.digikey.com/en/products/detail/sullins-connector-solutions/PPPC042LFBN-RC/810244) or 2 strips of 8 | 1 | for motors |
| 7 female header pins | | 2 | for QT Py |
| 8 male header pins | | 4 | for servos |
| battery wires | JST RCY OR 9V battery snap | 1 | [Amazon JST RCY](https://www.amazon.com/dp/B00Z04QFN2/) |
| servo buck boost 5v 2A OR replace with a short length of wire| [Pololu](https://www.pololu.com/product/4085) | 2 | regulators are needed if you want to supply voltages above or below what servos can accept. There are 2 servo power buses, each with 4 servos. |

![front view](https://github.com/RCMgames/RCM-Hardware-BYTE/blob/67634be8aeb1c3cb82b1d1cb7a75f85f452896bf/photos/P1040746.JPG)
![back view](https://github.com/RCMgames/RCM-Hardware-BYTE/blob/67634be8aeb1c3cb82b1d1cb7a75f85f452896bf/photos/P1040747.JPG)

## Acknowledgements
* I would like to thank [PCBWay](https://www.pcbway.com/) for sponsoring prototyping runs of this project. PCBWay produces very nice boards, supports open source hardware, and gave me great support as I worked onthis project. Special thanks to Liam!
