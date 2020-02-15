# smart-usb-switch

An inline USB type-A power switch that's controlled by an ESP8266 (ESP-12F) on
GPIO4. You can load this device with any firmware you want, including for
example [ESPHome](https://esphome.io).

Version 2 has two buttons on the back. If you build this board yourself, you can
put 0, 1, or 2 of the button components in place.

The PCB could probably be a little smaller, but the ESP-12F takes up a lot of
real estate.

## How to program

These instructions are for ESPHome, but since it's just an ESP8266, you can do
anything you want instead.

Soldering jumper pins on the terminal points is optional. Get ESPHome ready with
a .yaml file like the one included in this project. Connect the PROG terminals
to each other. Using a USB-TTL adapter _that is configured to use 3.3-volt logic
levels_, connect GND, 3V3, TX, RX (in other words, match up the labels on the
USB-TTL adapter with the ones on the smart switch, but connect RX to TXD and TX
to RXD). Then build the ESPHome image and upload with
`esphome your-config.yaml run` or however else you use ESPHome.

## Bill of Materials

See `smart-usb-switch.csv`.
