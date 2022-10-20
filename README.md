# VOID9
*A 3x3 handwired macropad*

![VOID9](https://i.imgur.com/Db82OaX.jpg)

The VOID9 is a 3d printed, handwired, 4x4 macropad running QMK Firmware on a Pro Micro controller.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is(if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the threads might get stripped.

# Breaking changes

WARNING: The pins mentioned in the guide for the VOID9 are not correct; they've been recently swapped, use the column pinout mentioned below instead (pins D1, D4, D0), or if you have an older build of the macropad (which was using pins D1, D0, D4) edit the info.json file in the qmk fork in order to reflect your wiring!

# Bill Of Materials

* 3d printed case parts
* 9 x Cherry MX style mechanical switches
* 9 x diodes ([tme.eu](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/))
* 9 x keycaps of choice
* 1 x Pro Micro ([Aliexpress](https://www.aliexpress.com/item/32902569443.html))
* 0.5 mm wire
* hotglue
* 4 x M3x10 Allen head bolts ([tme.eu](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/) / 13mm overall length, 5,5mm diameter head)
* 4 x 8mm bumpons

# Handwiring guide

I've also put together a pretty visual handwiring guide for the VOID9, that you can browse over [here](https://victorlucachi.ro/journal/void9-wiring-guide/).

| ![](https://i.imgur.com/01WknB5.jpg) 	| ![](https://i.imgur.com/GMMczAH.jpg) 	| ![](https://i.imgur.com/5NyUoJY.jpg) 	|
|---------------------------------------	|---------------------------------------	|---------------------------------------	|

# Pin assignment

    ROW0    ROW1    ROW2
    F4      F5      F6
    
    
    COL0    COL1    COL2
    D1      D4      D0
    
    Encoder Pad A           Encoder Pad B
    B1                      F7
    B2                      B3

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/dev_void/keyboards/handwired/void9). Edit them to suit your own needs and build the firmware following the QMK docs.

If you plan on using the VIA keymap dont forget to download the json definitions file linked in this repository.

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).
