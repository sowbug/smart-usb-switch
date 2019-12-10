smart-usb-switch
===

An inline USB type-A power switch that's controlled by an ESP8266
(ESP-12F) on GPIO14. You can load this device with any firmware you
want, including for example [ESPHome](https://esphome.io).

Program with a serial adapter that's set to 3.3v logic
levels. Remember to close the FLASH jumper on powerup if you want to
boot into programming mode.

Current big bugs:

- The USB plug footprint doesn't quite fit the component. I sanded and
  scraped until it did.

- On powerup, the MOSFET allows current through. So the connected
  device flashes for a moment when the switch is first plugged in.

The PCB could probably be a little smaller, but the ESP-12F takes up a
lot of real estate.
