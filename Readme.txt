Revision 1.2 (?) ******* CvW's Changes *******
Use second button to switch between leaded and unleaded solder temperature profiles. User gets confirmation via LCD.
Since rates of change between Leaded and unleaded solder profiles are similar, I left the PID constants alone.

Added error message in case initial oven temperature is too high - before, aborted start failed silently.
Added fan support - fan comes on with oven and turns off once interior temperature is low enough at the end of the cycle
I did not attempt to move switch monitoring to an ISR or fix the potential millis() rollover problem. Neither issue seems to be that pressing. 

Oh, and while the reflow controller file is saved as a .pde file here, you will need to rename it with a .ino extension if you want to use it with Arduino IDE 1.0 and up. This is my first contribution to GitHub, I hope I followed proper procedure. Cheers, CvW.

Revision 1.1 ****** Readme from Rocket Scream team: ******
1. Please use the Diptrace version 2.2 and above to open/edit the schematic & layout file. 
Newer files are not backward compatible with older version of Diptrace.
2. Hardware version 1.30 & 1.40 is 100% compatible and has component packages changes only.
3. In order to use the sketch in Arduino 1.0, please use the latest Arduino PID Library and the MAX6675 Library from Adafruit. Both libraries are available on GitHub.

