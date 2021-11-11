# Panasonic Wifi Module

This is a hardware module designed to plug into the CN-CNT connector on compatible Panasonic Airconditing Units

This is designed to run the esphome-panasonic-ac ESPHome library created by DomiStyle (https://github.com/DomiStyle/esphome-panasonic-ac) and all credit for the software goes to DomiStyle and other contributors.  

A cable with a 5 pin JST PA connector on one end and a 4 pin Molex PicoBlade on the other is required.  The 12V from the CN-CNT connector is unused so is not connected.  You can buy 4 pin pre-crimped PicoBlade cables from the likes of Adafruit - crimping tiny connectors can be challenging so buying a pre-crimped tail and soldering it to longer wires with a JST PA connector on the other end is a good option.

Programming is done using a 6 pin programmer.  Any programmer which adheres to the ESPFlash convention should work.  A programmer designed by myself is available at https://go.jmn.id.au/espprog but there are others (e.g. [SuperHouse ESPF](https://github.com/SuperHouse/ESPF)).  Alternatively any serial adapter can be used, but the ESP32 will need to be put into boot mode manually by pulling GPIO0 to ground during startup.

The smallest component is the 0603 capacitors and resistors so with a steady hand it's not too difficult assembling by hand and reflowing with a toaster oven, frypan or similar.  Using a solder paste stencil is easier but it wouldn't be too hard to dispense the solder manually too.

This was developed in KiCAD 5.99 so the latest nightly build should be used until KiCAD 6 is formally released.

![assembled board](/Assembled_board.jpg "Assembled Board")