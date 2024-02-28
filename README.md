# ESPHOME-RGBLight

I created a small device to control my WS2812b RGB Led strips.

![](https://github.com/WaarlandIT/ESPHOME-RGBLight/blob/main/RGBLight-controller.jpeg?raw=true | width=300)

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

Then use ESPHome to build the binary and write it to the ESP-01s.


