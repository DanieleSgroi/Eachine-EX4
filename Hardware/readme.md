# Hardware

This repository contains some images of the DF806B Hardware.

It also provides some commented images to explain some hackings referenced.

# USB Interface

On Flight Controller bottom side, there is a spare unused connector which turned out to be an USB interface (see image EX4-BOT-DFU).

This connector mates with MOLEX 0511460400 shell and MOLEX 0506418141 pins, however pre assembled cables may be found on Aliexpress: https://aliexpress.ru/item/4000586964114.html

This USB interface is useful to connect to Mission Planner for parameter adjustments and to update the Flight Controller Firmware throug DfuSe.

# BOOT 0 PIN 

The BOOT 0 pin shall be tied to +3V3 at boot in order to put the STM32F405 CPU in DFU mode, required for firmware upload. This can be accomplished by temporary connection between the highlited red solder pins (see image EX4-BOT-DFU). 
