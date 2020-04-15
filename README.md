# mitsubishi2MQTT
Use MQTT and ESP8266/ESP32 module to control Mitsubishi HVAC unit.
It use SwiCago librairies: https://github.com/SwiCago/HeatPump

***
Features:
 - Configured for domoticz mitsubishi mqtt python plugin.
 - Respects swicago mqtt implementation and example.
 - Works http control wtihout mqtt.
 - Initial config:  WIFI AP mode and web portal.
 - Web interface for configuration, status and control, firmware upgrade.
 

***
Screenshots:

Main Page
![](https://github.com/gysmo38/mitsubishi2MQTT/blob/master/images/main_page.png)

Control page
![](https://github.com/gysmo38/mitsubishi2MQTT/blob/master/images/control_page.png)

Config page
![](https://github.com/gysmo38/mitsubishi2MQTT/blob/master/images/config_page.png)

***
How to use:
 - Step 1: flash the sketch with flash size include SPIFFS option.
 - Step 2: connect to device AP with name HVAC_XXXX (XXXX last 4 character MAC address)
 - Step 3: You should be automatically redirected to the web portal or go to 192.168.1.1
 - Step 4: set Wifi information, save & reboot. Fall back to AP mode if WiFi connection fails (AP password sets to default SSID name from step 2).
 - Step 5: find the device IP with last 4 character MAC address in your router
 - Step 6: (optional): Set MQTT information for use with Home Assistant
 - Step 7: (optional): Set Login password to prevent unwanted access in SETUP->ADVANCE->Login Password
