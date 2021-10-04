# Panasonic Wifi Module

This is a hardware module designed to plug into the CN-CNT connector on compatible Panasonic Airconditing Units

This is designed to run the esphome-panasonic-ac library created by DomiStyle (https://github.com/DomiStyle/esphome-panasonic-ac) and all credit for the software goes to DomiStyle and other contributors.  

A cable with a 5 pin JST PA connector on one end and a 4 pin Molex PicoBlade on the other is required.  The 12V from the CN-CNT connector is unused so is not connected.

Programming is done using a 6 pin programmer.  Any programmer which adheres to the ESPFlash convention should work.  A programmer designed by myself is available at https://github.com/jnicolson/espprog but there are others.  Alternatively any serial adapter can be used, but the ESP32 will need to be put into boot mode manually by pulling GPIO0 to ground during startup.