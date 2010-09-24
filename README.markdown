
This is an ATmega328-based (Arduino-compatible) daughterboard for the
Dragino board (http://www.dragino.com/?p=21). This daughterboard includes
a socket for an XBee radio module, as well as a 16-pin box header (for an
IDC ribbon cable connector) to connect up a standard HD44780 LCD display
module, along with the AVR microcontroller.

The Dragino board can throw a reset to the AVR by taking GP0 high, which
means that a new Arduino sketch can be uploaded through the UART, if the
appropriate tools are installed on the Dragino board.

A DS18B20 temperature sensor is also installed on the board.

The Dragino's external 12-pin interface terminal block is connected to the
reset line and the SPI pins on the AVR, as well as the ADC input channels.
This means that ICSP programming of the AVR can be performed using a
standard ICSP programmer, with an appropriate cable made up to plug the
programmer into the 12-pin terminal block.

A set of current sensors (with appropriate analog front-end circuits) can
be plugged into the external interface port too, and/or a resistive
touchscreen such as the Nintendo DS style low-cost touchscreen, and a LDR.

I don't have access to a Dragino board at this stage, and I had to take the
measurements for the footprint of the Dragino header pins from the layout
of the Flukso-meter daughterboard.

I haven't double checked the layout of these pin headers yet, though, and
this needs to be checked before boards are manufactured. It also needs to be
checked more generally once I have a look at a Dragino board, too, to ensure
that the board is not too wide, and clears the other components (such as the
ethernet RJ45 jack) once it is plugged into the Dragino motherboard.





















