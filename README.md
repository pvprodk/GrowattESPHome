# GrowattESPHome
ESPHome based code for Growatt inverters

# Description
The code (growatt.yaml) can be used on a ESP8266 with a TTL-to-RS485 adapter, or by putting the Growatt ShineWifi-X into boot mode and flashing it with ESPHome.

# Using the ShineWifi-X
To flash the ShineWifi-X with ESPHome you need to put it into boot mode, by jumping the GPIO0 and GND pins while plugging in/powering on the USB-device. Important to remove the jumper before you flash:
![These pins need to be shorted to put the ShineWifi-X into boot mode](https://i.imgur.com/IZa4ood.jpg)

# Using a ESP8266
You can also build you own, using a ESP8266 and a TTL-to-RS485 adapter, based on the scematics below (credit to [the author](https://www.youtube.com/watch?v=znwNZstQqYE))
![Diagram](https://i.imgur.com/jVm6FFr.png)
Be sure to edit the board type and pins to your specific configuration.
