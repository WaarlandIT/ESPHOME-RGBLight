# ESPHOME-RGBLight

I created a small device to control my WS2812b RGB Led strips. 12 volt led strips have less issues with voltage drop over large lengths. 
This device needs a 12 Volt power supply to power the lights, it has a voltage regulator to drop the voltage for the ESP-01s. 

![image](https://github.com/WaarlandIT/ESPHOME-RGBLight/assets/53364386/35758fe5-3988-4907-b47d-bbb3a9ef2fc8)


To add them to Home Assistant I prefer to make use of MQTT because the lights are not in the same network as Home Assistant is and the MQTT broker is reachable from every network I work with.
It is also possible to add it as a ESPHome device using the API call.

## How to use this device
You need to set some variables, I do that via the secrets file:
- api_key
- wifi_ssid
- wifi_password
- mqtt_server
- mqtt_user
- mqtt_password

And you need to set the amount of RGB Leds you have in your string. 

Then use ESPHome to build the binary and write it to the ESP-01s.

## Home Assistant usage
In Home assistant the property for the new device is like this
![image](https://github.com/WaarlandIT/ESPHOME-RGBLight/assets/53364386/8a183a75-69c2-4256-bc43-b918bb633ead)

You can change color and brightness like any other RGB light bulb. There is also a collection of 15+ different effects, this collection might grow when the community create more of these. 


