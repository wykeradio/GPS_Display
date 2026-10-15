# GPS_Display
A standalone GPS display device for your car or portable radio operation
Ideal for POTA/SOTA/145Alive etc..

You will require:
1 x Arduino (ATMEGA328)
1 x uBlox Neo-6 GPS Receiver (or any GPS Receiver that outputs NMEA Sentences on UART)
1 x 16x2 LCD Display (I2C)
Some Hookup Wire

DO NOT CONNECT THE GPS RX PIN TO ANY VOLTAGE - YOU WILL DAMAGE THE MODULE!
<img width="875" height="745" alt="wiring" src="https://github.com/user-attachments/assets/ef066b97-9001-490e-abce-cdb1d8524824" />


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
<img width="2560" height="1440" alt="power_on" src="https://github.com/user-attachments/assets/d79ad1ec-c1ff-4265-b2f8-59077c2cd5fd" />

The Acquiring of Satellites
<img width="2560" height="1440" alt="initial_search" src="https://github.com/user-attachments/assets/04b3b879-ae6d-4383-bbc6-1803be99a225" />

Locked in and displaying Lat and Long
<img width="2560" height="1440" alt="locked" src="https://github.com/user-attachments/assets/c6f21dff-07ec-43cd-a654-25b10c70fa72" />

Displaying Grid and number of Sats & Bearing
<img width="2560" height="1440" alt="grid_and_num" src="https://github.com/user-attachments/assets/c34fb96c-f7b2-4259-965c-6f0711e8ca43" />

For more details:
https://www.wavewizards.org/arduino/gps/




Every few seconds the display will change to show Grid (Maidenhead Locator)
The number of Satellites the unit is receiving and if you are moving, your Bearing.


