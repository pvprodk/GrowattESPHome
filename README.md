# GrowattESPHome
ESPHome based code for Growatt inverters, in this example used with Home Assistant.



# Description
- The code (growatt.yaml) can be used on a ESP8266 with a TTL-to-RS485 adapter, or by putting the Growatt ShineWifi-X into boot mode and flashing it with ESPHome.
- This configuration pulls data every 5 seconds, feel free to adjust to your likings.
- Please note that there are two protocol_versions. Newer Growatt inverters, that comes with a ShineWifi-X uses RTU2. Older versions use RTU.
- This code is tested on Growatt MOD XXXTL3-X and SPHXXXXTL3 BH UP
- ESPHome 2022.4.0 or newer required

# Using the ShineWifi-X
To flash the ShineWifi-X with ESPHome you need to put it into boot mode, by jumping the GPIO0 and GND pins while plugging in/powering on the USB-device. Important to remove the jumper before you flash:

![These pins need to be shorted to put the ShineWifi-X into boot mode](https://i.imgur.com/IZa4ood.jpg)

# Using a ESP8266
You can also build you own, using a ESP8266 and a TTL-to-RS485 adapter, based on the scematics below (credit to [the author](https://www.youtube.com/watch?v=znwNZstQqYE))

![Diagram](https://i.imgur.com/jVm6FFr.png)

Be sure to edit the board type and pins to your specific configuration.
Remember to terminate the RS485 circuit with a 120ohm resistor
