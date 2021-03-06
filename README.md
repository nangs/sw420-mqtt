# Vibration sensor - SW420

> This LUA script is for ESP8266 hardware.

## Description

Send SW420 data (level and amplitude) through an ESP8266 to a MQTT broker.

## Files

* ``config.lua``: Configuration variables
* ``init.lua``: Connect to a wifi AP and then execute main.lua
* ``main.lua``: Main file

## Principle

1. Connect to a wifi AP
2. Start a MQTT client and try to connect to a MQTT broker
3. Publish data (level and amplitude) to MQTT broker each time GPIO changes level

## Scheme

![scheme](https://github.com/Wifsimster/sw420-mqtt/blob/master/scheme.png)
