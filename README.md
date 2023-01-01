# dsmr-swe - Main
ESPHome configuration for the built in DSMR Component, Swedish translation

This is my cofiguration file for a wifi-P1/HAN-reader using the built in DSMR-component in ESPHome. 
There are multiple resources available on GITHub that covers hardware and different approaches. My contribution is sorting out the OBIS-codes used and a Swedish translation of the metering component according to the swedish DLMS protocol.

Feel free to reuse the code according to the license!

/MickeWHR

## Hardware used:
Kamstrup Omnipower with the "HAN-P1" module
(Baud-rate 115200 and you need to supply power to the module through the P1 port)

Slimmelezer+ by Zuidwijk
https://github.com/zuidwijk/dsmr

RJ12-extender connector with soldered connection to a 5V USB-cable, provides power to the Slimmelezer and P1-module.

## Disclaimer
There is a Light branch that I use since I'm only interested in those sensors.

Reactive power in/out does not work for my meter. (2022-12-08) I think that the built in DSMR parser doesn't recognize kVArh/kVAr instead of kvarh/kvar.

This guy has solved everything with his own parser:
https://github.com/psvanstrom/esphome-p1reader

A LOT of information is available on the official ESPHome site:
https://esphome.io/
