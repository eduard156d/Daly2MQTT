# Daly2MQTT [![GitHub release](https://img.shields.io/github/release/softwarecrash/Daly2MQTT?include_prereleases=&sort=semver&color=blue)](https://github.com/softwarecrash/Daly2MQTT/releases/latest) [![Discord](https://img.shields.io/discord/1007020337482973254?logo=discord&label=Discord)](https://discord.gg/fb2nZWDExz)
Little Program for ESP82XX to get the Daly BMS data to web and MQTT

# Features:
- captive portal for wifi and MQTT config
- config in webinterface
- switching MOS gates over webinterface, MQTT and via web at /set?loadstate, set SOC over MQTT
- get essential data over webinterface, get all data like cell voltage and more over MQTT
- classic MQTT datapoints or Json string over MQTT
- get Json over web at /livejson?
- firmware update over webinterface
- debug log on Wemos USB (use only if you **don't** supply Wemos from BMS!!!)
- wake the BMS over MQTT or keep it awake (not supported on ESP-01s)
- universal switching output (only with external power supply, not supported on ESP-01s)
- [blink codes](https://github.com/softwarecrash/Daly2MQTT/wiki/Blink-Codes) for the current state of the ESP (not supported on ESP-01s)
- with Teapod


**Main screen:**

![grafik](https://user-images.githubusercontent.com/17761850/227793485-cdc02fcf-d10e-471e-a1d9-a0fc15785f66.gif)
---
  
![Daly-Cells](https://github.com/softwarecrash/Daly2MQTT/assets/17761850/d16ea396-db2d-427f-9f68-13151c13d22d)


**Settings:**

![grafik](https://user-images.githubusercontent.com/44615614/212401754-81a16130-f24d-4c8a-babc-d18d112fad5a.png)


**Config:**

![grafik](https://user-images.githubusercontent.com/17761850/227793333-5e51fc9b-d535-4345-882c-adb758e8bf6d.gif)


**MQTT Data**

![grafik](https://user-images.githubusercontent.com/44615614/161782578-aabdde4d-4f51-4312-9392-9fdf4d45df24.png)


# How to use:
- flash the bin file to an ESP8266 (recommended Wemos D1 Mini) with [Tasmotizer](https://github.com/tasmota/tasmotizer/releases) or use the [Online Flash tool](https://softwarecrash.github.io/Daly2MQTT/espflashtool/)
- connect the ESP like the [wiring diagram](https://github.com/softwarecrash/Daly2MQTT/wiki/Wiring)
- search for the wifi ap "Daly2MQTT-AP" and connect to it
- surf to 192.168.4.1 and set up your wifi and optional MQTT
- that's it :)

# External links

[Here you can find the communication methods for your BMS](https://www.dalyelec.cn/newsshow.php?cid=24&id=65&lang=1)

[Collection of docs, software and firmware around Daly BMS](https://github.com/all-solutions/DALY-docs-soft-firm). **Firmware-Updates are at your own risk! NO SUPPORT!**

# Completely assembled and tested PCB's

You are welcome to get fully stocked and tested PCB's. These are then already loaded with the lastest firmware. The earnings from the PCBs are used for the further development of existing and new projects.

![Daly-BMS-MQTT-PCB](https://user-images.githubusercontent.com/17761850/233857094-38f22d6f-4d74-4643-b426-182fc4dc9a44.png)

If interested see [here](https://all-solutions.store)

**NEW:** The new PCB's (v2) are now completely galvanically isolated from the BMS when operating with an external power supply.

#
[<img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"/>](https://donate.softwarecrash.de)
# 
[![LICENSE](https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
