# GPS_Display
A standalone GPS display device for your car or portable radio operation
Ideal for POTA/SOTA/145Alive etc..

You will require:
1 x Arduino (ATMEGA328)
1 x uBlox Neo-6 GPS Receiver (or any GPS Receiver that outputs NMEA Sentences on UART)
1 x 16x2 LCD Display (I2C)
Some Hookup Wire

DO NOT CONNECT THE GPS RX PIN TO ANY VOLTAGE - YOU WILL DAMAGE THE MODULE!

Connect the LCD Display to the Arduino:

Display         Arduino

GND             GND on Arduino
VCC             5V
SDA             SDA
SDL             SDL


Connect the GPS Receiver

GPS Pin         Arduino Pin
VCC             3V3
RX              Leave Disconnected
TX              4 (Fifth pin in)
GND             GND

Program the Arduino.
Reboot Arduino

You should have no problems when using the unit outside or near a window inside.
For better sensitivity you can use an Active Antenna

The Display will show a short Splash Screen

The Acquiring of Satellites

Locked in and displaying Lat and Long

Every few seconds the display will change to show Grid (Maidenhead Locator)
The number of Satellites the unit is receiving and if you are moving, your Bearing.


