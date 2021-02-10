# Arduino OLED FHT Spectrum Analyzer

Arduino based Spectrum Analyzer with an .96" OLED display (SSD1306).  
Button used to switch between different bar sizes 12, 8, and 6.
Speaker input used for signal.  

This is a reworking of the forked project completed by uxking.
The target hardware for this project is an arduino model 2650 and 128x32 SSD1306

# Significant Software changes..
(Originally) FHT library for frequency spectrum analyser http://wiki.openmusiclabs.com/wiki/ArduinoFHT  
(Updated)  implemented using  version 4 of the FHT library dowloaded directly from OML URL above.

(Originally) Utilized U8glib.h for the display.  
(Updated)  Implemented new U8 library offering support for a larger variety of output devices

(Originally) Using GreyGnome's PinChangeInt to change detect button push and change number of bars displayed: 
     https://github.com/GreyGnome/PinChangeInt 
(Updated)  PinChangeInt deprecated.  Upgraded to use new version of interrupt library


# Attributions

https://github.com/uxking/Arduino_OLED_FHT_U8gLib_Spectrum_Analyzer  The basis for this work

(from the original readme)
Also found some code by the-fuchs on Github to help with the peak hold display. 
I believe his code was working with an MSGEQ7 7 band chip, but I was able to use some of his magic in my sketch.  
https://github.com/the-fuchs/AVR-7-BandAudioSpectrum check out main.c and his drawDouble or drawSingle functions.
