# esp8266ferraris
use an esp8266 and tcrt5000 to read ferraris meter and send to server system

This is my setup to read my Ferraris called power meter from the 80s which is using a spinning disk in silver with a red marker.
On the power meter should be a note how many turns represent 1kwH.

To read the spins of the disk I use a TCRT5000 IR track sensor.
You can get these online for about 2$.
You can buy these complete with a little potentiometer to set the sensivity and with 4 pin - connectors for V+, Ground, DigitalOut,
AnalogOut.

To send the read data to a server with a HTTP GET Request (in my case PIMATIC, a home automation control system, see here: www.pimatic.org)
I use a esp8266 NodeMCU V3 ESP-12, these come in many different versions, for about 5$.
They have wifi on board and can be programmed with the Arduino enviroment.

I used Arduino 1.65 & ESP Board Package 2.0.0, but newer versions might work too.

You will need the following libraries:
ESP8266WiFi.h
ESP8266HTTPClient.h
Base64.h
elapsedMillis.h

