**Arduino Code**

These Arduino code were written by Kevin Darrah: http://www.kevindarrah.com/?cat=99

Revision Notes:
Rev 7 ¨C First released code.  This is what you see running in the demo video, and all the tutorial videos

Rev 11 ¨C Fixed a bug in the Bit Angle Modulation, See the video How it Really Works for more information

Rev 12 ¨C Fixed the Bitwise Operation to set pins LOW.  I was doing it PORTX &= 0<<pinNumber, it should be PORTX &= ~(1<<pinNumber)  The wrong way was ANDing every pin in the port with 0, where is the new way ANDs only the pin you want to turn OFF with 0 and the rest with 1.