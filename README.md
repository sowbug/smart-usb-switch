smart-usb-switch
===

An inline USB type-A power switch that's controlled by an ESP8266
(ESP-12F) on GPIO14. You can load this device with any firmware you
want, including for example [ESPHome](https://esphome.io).

Program with a serial adapter that's set to 3.3v logic
levels. Remember to close the FLASH jumper on powerup if you want to
boot into programming mode.

At the moment, the known bugs from the first spin of the PCB are fixed,
but I haven't yet respun the PCB to verify the fixes.

The PCB could probably be a little smaller, but the ESP-12F takes up a
lot of real estate.
