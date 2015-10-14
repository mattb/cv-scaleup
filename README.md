# Control voltage step-up module

DC-coupled audio interfaces, such as the [MOTU 828 MkI](http://www.soundonsound.com/sos/jul01/articles/motu828.asp)
that I own, are capable
of [outputting voltages](http://www.expert-sleepers.co.uk/siwacompatibility.html) that can
control audio hardware such as
[Eurorack](http://electronicmusic.wikia.com/wiki/Eurorack) modules. However,
most Eurorack modules expect a CV range of -5v to 5v. I measured the MOTU as
outputting -2.88v to 2.88v.

This project contains Eagle files for a Eurorack-mountable opamp circuit with a gain that will
scale four MOTU outputs to the full CV range. It uses a single TL074 quad
op-amp and a few resistors. Calculations for the resistors were made using the calculator at 
http://earmark.net/gesr/opamp/gain_offset.htm

There is also a rudimentary 8HP front panel design in an Illustrator template.

As of October 13th 2015, PCBs have been ordered from OSHPark and panels from
Ponoko but have not yet arrived.  A single channel has been successfully tested on a
breadboard, and used to correctly track over 8 octaves of pitch control on
an Arturia Microbrute using Silent Way's Voice Controller plugin in Ableton Live.
