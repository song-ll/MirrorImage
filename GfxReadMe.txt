This is a library for our Monochrome Nokia 5110 LCD Displays

  Pick one up today in the adafruit shop!
  ------> http://www.adafruit.com/products/338

These displays use SPI to communicate, 4 or 5 pins are required to  
interface

Adafruit invests time and resources providing this open source code, 
please support Adafruit and open-source hardware by purchasing 
products from Adafruit!

Written by Limor Fried/Ladyada  for Adafruit Industries.  
BSD license, check license.txt for more information
All text above must be included in any redistribution

To download. click the DOWNLOADS button in the top right corner, rename the uncompressed folder Adafruit_PCD8544. Check that the Adafruit_PCD8544 folder contains Adafruit_PCD8544.cpp and Adafruit_PCD8544.h

Place the Adafruit_PCD8544 library folder your <arduinosketchfolder>/libraries/ folder. You may need to create the libraries subfolder if its your first library. Restart the IDE.

You will also have to download the Adafruit GFX Graphics core which does all the circles, text, rectangles, etc. You can get it from
https://github.com/adafruit/Adafruit-GFX-Library
and download/install that library as well 


Bitmaps of 48 fonts now consume 110073B / original 179672 B.
Bits of rows are XORed, there is a lot of zeros then and they are replaced by 0 bit in data 
(remaining non-zeros data use 9 bits).
Data are placed in a new container (cArrayPtr.h) during encoding, fixed 8 bits are followed by 
non-zero bytes (zeros are skipped), so best option is 0x00 for 8 zeros in a row and worst 0xFF and 8 
non-zero bytes.
Encoder is there:
https://github.com/eltomjan/ETEhomeTools/blob/master/gfxXorPacker.cpp
Developed and tested on my ArduinoSimulator 1st and then in Pololu A-Star 32U4 Micro & 
Adafruit_ILI9340 today.










Contact GitHub API Training Shop Blog About
© 2017 GitHub, Inc. Terms Privacy Security Status Help



