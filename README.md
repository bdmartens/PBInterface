# PBInterface
Pixelblaze v3 interface board/box
These are all the files I used to make a pixelblaze v3 controller interface board and controller box.
My intended purpose was an interactive project box for my kids.

The PCB allows interfacing with the board hard button (used to toggle between patterns, fairly hard-coded to the project), as well as GPIO 25 and 26 - which are pulled to ground by a button press.
It also exposes GPIO33, which allows for analog read.  Using a 102 trim pot resistor, this can be is pulled up to 3.3v.  My use case was with a pressure-sensitive strip, to be used as a mattress pressure sensor, so that my kids could make patterns that interacted with them being in their bed or not.

There is also place for an electrolytic capacitor - not sure if it is needed, but I went with a fairly beefy 1000 uf cap to keep power even given my amazon-purchased power supply.

The hard button and GPIO 33 are only accessible via a contact pad on the back of the pixelblaze v3, and as such would need to be hand-soldered via a wire between the pixelblaze and the interface board. 

Otherwise, solder header pins in for th epower connection, reset/hard button, and button 25/26.  I have a terminal block on mine to connect to the sensor strip (in the photo, hidden under the power socket wires)
There is also a header for a power switch, which I use a mini toggle switch.

I have also included the fusion 360 PCB box project file, as well as a step file, with most of the parameters set as variables that can be modified as needed.
The box holes are sized to hava M2 bolts used, but this can also be modified in the fusion 360 parameters.
