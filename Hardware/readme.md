# Hardware

This repository contains some images of the DF806B Hardware.

It also provides some commented images to explain some hackings referenced.

# USB Interface

On Flight Controller bottom side, there is a spare unused connector which turned out to be an USB interface:

![USB](./EX4-BOT-DFU.jpg) 

This connector mates with MOLEX 0511460400 shell and MOLEX 0506418141 pins, however pre assembled cables may be found on Aliexpress: https://aliexpress.ru/item/4000586964114.html

When connected to a PC, this nterface exposes a COM port operating at 115200,8N1. This USB interface is useful to connect to Mission Planner for parameter adjustments and to update the Flight Controller Firmware throug DfuSe.

# BOOT 0 PIN 

The BOOT 0 pin shall be tied to +3V3 at boot in order to put the STM32F405 CPU in DFU mode, required for firmware upload. This can be accomplished by temporary connection between the highlited red solder pins.. 

# Spare Serial Port

On top side, close to the power switch connector, there is an unpopulated area for the Optical Flow connector (4 pin, not installed on DF806B).


![TOP](./EX4-TOP-MB.jpg) 

This is suspected to be a spare serial port and may be useful for further expansions (e.g. 3DR telemetry, Airborne Mission Computer, etc.).

TO BE FURTHER INVESTIGATED.

# BATTERIES

EX4 batteries are LiHV type and can be charged up to 4.35 Volts per cell. Pack configuration is 3S, so up to 13.05 Volts. 

I've modified a stoch charger to allow operation with an Imax B6 charger, also modified with cheali-charger firmware: https://github.com/stawel/cheali-charger to support LiHV cells.

![B6](./IMAX-B6.jpg) 

The copper layer helps to improve the thermal conductivity between the battery pack and the embedded LM35 temperature sensor, to allow monitoring of temperature during the charge process.

With this setup I can fast charge, balace and discharge to storage the batty pack. Hope to increase battery life!

