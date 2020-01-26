
<p align="center">
  <img src="https://github.com/home-assistant/home-assistant-assets/blob/master/loading-screen.gif">
</p>

These are the [Home Assistant](https://home-assistant.io/) configuration files used in my Home Assistant (HA) setup. I relied on repositories of other HA users quite a bit when I was getting started for ideas and example code.  Hopefully this repository will help someone else who is getting started. 

# Automations:
A detailed description of each of my automations and a link to the yaml file is located [HERE](https://github.com/SilvrrGIT/HomeAssistant/tree/master/automation#automations)

This is the most important part of Home Assistant!  Remote control and voice commands are nice, however, that is not home automation, just remote control.  Automations should make your life easier, look at what you do every day, the simplest things, and automate them.  To me Home Automation is collecting data about your home and automatically acting based on that data.

# My Home Assistant Setup:

I run my home assistant instance on a Zotac mini PC.  The previous life of this device was as a Datto Alto2 backup solution.  It has a AMD GX-415GA quad core processor, 8GB of RAM, 64GB SSD and sips on power.  The base operating system is [Ubuntu Server 18.04.3 LTS](https://ubuntu.com/download/server) and it runs [Hass.io via docker](https://www.home-assistant.io/hassio/installation/#alternative-install-on-a-generic-linux-host). It also runs the following add-ons. 

* [Adguard Home](https://github.com/hassio-addons/addon-adguard-home)
* [Backup to Google Drive](https://github.com/sabeechen/hassio-google-drive-backup)
* [Mosquitto MQTT broker](https://www.home-assistant.io/addons/mosquitto/)
* [Network UPS Tools](https://github.com/SilvrrGIT/hassio-addons)
* [RPC Shutdown](https://www.home-assistant.io/addons/rpc_shutdown/)
* [SSH](https://www.home-assistant.io/addons/ssh/)
* [Samba](https://www.home-assistant.io/addons/samba/)
* [Unifi Controller](https://github.com/hassio-addons/addon-unifi)
* [VScode](https://github.com/hassio-addons/addon-vscode)

I'm currently running [Home Assistant](https://home-assistant.io) version __0.104.2__ on this instance.

# UI Based Integrations:
The following integrations are setup in the User Interface (UI) and may be a missing peice as to the full configuration of my HA setup. 

* [Adguard Home](https://www.home-assistant.io/integrations/adguard/)
* [IKEA Trådfri (Tradfri)](https://www.home-assistant.io/integrations/tradfri/)
* [MQTT](https://www.home-assistant.io/integrations/mqtt/)
* [Unifi Controller](https://www.home-assistant.io/integrations/unifi/)
* [Google Cast](https://www.home-assistant.io/integrations/cast/)
* [iOS](https://www.home-assistant.io/integrations/ios/)
* [Zone](https://www.home-assistant.io/integrations/zone/)
* [ZWave](https://www.home-assistant.io/docs/z-wave/installation)

# A Few Stats On my Setup:
| Tracked Devices | Lights | Binary Sensors | Switches | Automations | Scripts | Sensors | Zwave Devices |
|:---------------:|:------:|:--------------:|:--------:|:-----------:|:-------:|:-------:|:-------------:|
|45               |14      |6               |40        |81           |6        |156      |10             | 

# Connected Devices:

### Cloud Controlled Devices:

* [Google Nest Hub](https://store.google.com/us/product/google_nest_hub) Used for voice commands to turn devices on/off and casting a view with a few switches
* [iPhone 11](https://www.apple.com/iphone-11/) Used for presence detection

### Wifi Connected Devices
* [Xiaomi Yeelight RGBW E27 Smart LED Bulbs](http://www.gearbest.com/smart-lighting/pp_361555.html) *
* [Xiaomi Yeelight E27 Smart LED Bulbs](http://www.gearbest.com/smart-light-bulb/pp_278478.html) *
* [Broadlink RM Mini 3](https://www.amazon.com/BroadLink-Control-Universal-Remote-RMMINI3-EN/dp/B01FK2SDOC/ref=sr_1_2?ie=UTF8&qid=1499475366&sr=8-2&keywords=broadlink+mini3)*
* [Sonoff Basic (Flashed with Tasmota)](https://www.amazon.com/Sonoff-Wireless-Modified-Low-cost-Compatible/dp/B06WWNBD3Y?ref=ast_p_ei)*
* [Sonoff POW (Flashed with Tasmota)](https://www.amazon.com/Sonoff-Consumption-Monitoring-Appliances-Compatible/dp/B06XSD6PD6?ref=ast_p_ei)*
* [Sonoff TH16 (Flashed with Tasmota)](https://www.amazon.com/Sonoff-TH16-Temperature-Monitoring-Compatible/dp/B06XTNSJ46)*
* [OpenGarage Door Controller ](https://www.amazon.com/OpenGarage-WiFi-enabled-Garage-Door-Opener/dp/B01M4RL0CL)*
* [Kuled WiFi Light Switches (Flashed with Tasmota)](https://www.amazon.com/Required-Wireless-Requires-Schedule-Compatible/dp/B079FDTG7T)*
* [Firefly Electronix Wifi Doorbell](https://www.fireflyelectronix.com/product/wifidoorbell)*

### Zwave / Zigbee Devices
* [Ikea TRÅDFRI LED Bulbs](http://www.ikea.com/us/en/catalog/products/20318267/)
* [Ikea TRÅDFRI Remote](http://www.ikea.com/us/en/catalog/products/20303317/)
* [Mono Price Z-wave Door Tilt Sensor ](https://www.monoprice.com/product?p_id=11987)
* [GE Z-Wave Plus Hinge Pin Door Sensors ](https://www.amazon.com/GE-Wireless-Attaches-Existing-32563/dp/B01KQDIUAW/)
* [Aeotec Z-wave Range Extender ](https://www.amazon.com/Aeotec-Range-Extender-Z-Wave-repeater/dp/B01M6CKJXC)
* [Dome Miniature, Z-Wave Plus Door/Window Sensor](https://www.amazon.com/Dome-Home-Automation-Miniature-DMWD1/dp/B01JGMZNNG)
* [Go Control Thermostat](https://www.gocontrol.com/detail.php?productId=3)
* [Aeotec Home Energy Meter Gen2 ](https://aeotec.com/z-wave-home-energy-measure/)
* [Zooz Z-wave Dimmer Switches ](https://www.amazon.com/Z-Wave-Switch-Existing-Switches-Add-Ons/dp/B07K37BNMC?th=1)

### Hardwired Devices
* [Cyberpower CP1500PFCLCD UPS ](https://www.amazon.com/CyberPower-CP1500PFCLCD-Sinewave-Outlets-Mini-Tower/dp/B00429N19W) used to detect power outages and keep network and HA running in a power outage.
* [Ubiquiti Unifi AP-AC Long Range - Wireless Access Point](https://www.ui.com/unifi/unifi-ap-ac-lr/) used for presence detection
* [Ubiquiti Unifi Security Gateway](https://www.ui.com/unifi-routing/usg/) used for network stats
* [Ikea TRÅDFRI Gateway](http://www.ikea.com/us/en/catalog/products/00337813/) *

*Block these from external network access and they will still work on your local network with Home Assistant.

# Front End Screen Shots:

## Home
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/rooms.png">
</p>

## Switches
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/switches.png">
</p>

## Device Status
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/devicestatus.png">
</p>

## Home Assistant Status
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/ha.png">
</p>

## Automations
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/automations.png">
</p>

## Data
<p align="center">
  <img src="https://raw.githubusercontent.com/SilvrrGIT/HomeAssistant/master/www/data.png">
</p>

# Questions?

The best way to get help on Home Assistant is the [Home Assistant Forum](https://community.home-assistant.io/).  If you have a specific question about my configuration send me a Private Message on the HA forum, my username over there is [Silvrr](https://community.home-assistant.io/u/silvrr/).  If you have found something incorrect, please submit an issue here on Github and I will get it fixed.
