## Open Access Control for SYN Shop


Based on version Open Access Control Mega Firmware 1.02.  Updated for SYN Shop Use.

Hardware is the Open Access Control 3.1 Mega

https://code.google.com/p/open-access-control/


## Compiling

Uses the Arduino IDE 1.5.5

Libraries have not been added yet for the on board AT24C EEPROM, so user data is being
stored in the Arduino Mega's interal EEPROM.  As a result when reprogramming, the Arduino
EEPROM data needs to be preserved to maintain access.


## Known Issues

* If we monitor more than one zone for motion, we have problems reading badges
* Front door badge reader gets occasional misreads, could be hardware on the reader, or
some buffer is partially getting filled and not cleared properly
* Reading button presses after read only works for two digits


## Todo

* Add library to move user data to AT24C
* Add code to read user pin after badge swipe for access


