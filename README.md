# Simple-Micropython-MLX90614-Library
A simple yet usable library for MLX90614 using Micropython. 

This library can be use to interface, configure, and read data from MLX90614 IR temperature sensors. This library is by no means optimized, it's written to be as readable as possible for new programmers. It is functional, but is not yet fully debugged, nor optimized. Use AS IS, I'm not resposible of any damages, misconfigurations, or anything caused by the use of this code. Use at your own risk. 

You can use this library to read temperature data from the sensor. You can write almost all configuration values to eeprom, such as emissivity value, filters and gains. 

Part of this library code was taken from the work of mcauser (https://github.com/mcauser/micropython-mlx90614), such as the crc8 implementation and dualzone detection. I wanted to make it simpler to read, and add all the configuration from the datasheet. There's a bit of work yet to be done, but most of the things you can do with this sensor are already implemented.

Things to be done:
* Debug...
* Flags...
* Sleep Mode...

This library was tested on a Raspberry Pi Pico. If you have issues reading data from this sensor, I highly encourage you to try this things:
* Assure that your power supply is supplying enough current/voltage.
* Check your pull up resistors.
* Use SoftI2C instead.

I will add more info as soon as possible. For now you can play with the script, I tried to make everything as readable as possible.
