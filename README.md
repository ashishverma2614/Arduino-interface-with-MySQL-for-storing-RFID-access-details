# Arduino-interface-with-MySQL-for-storing-RFID-access-details

You can check it's video at https://youtu.be/JQv7_nu6G8o and you can contact us at info [@] deligence.com in case you have any query. You can also contact us at sales [@] deligence.com in case of any Development requirement.

Here We are going to connect Arduino UNO, RFID (MFRC522) & Ethernet Shield with MYSQL Database. So for that first we should connect our Arduino Board with the Ethernet Shield & RFID Module.
By using the RFID Module we are going to scan our RFID card and tag which are allow or not. And by using our Ethernet shield we are going to send that data to our MYSQL Database which is connect through a pho page. Bellow we provided the code for PHP as well as for Arduino. You also can go through our video to better understanding how to create a database in MYSQL and how to connect with PHP and Arduino.


NOTE-BECAUSE WE ARE USING TWO SPI DEVICES THAT’S WHY WE HAVE TO CHANGE OUR SS PIN FOR RFID MODULE .
Pin Layout

https://github.com/DeligenceTechnologies/Arduino-interface-with-MySQL-for-storing-RFID-access-details/blob/master/RFID_LOGGER_WITH_MYSQL_DATABASE.docx?raw=true

ETHERNET SHIELD
The Arduino Ethernet Shield 2 connects your Arduino to the internet in mere minutes. Just plug this module onto your Arduino Board, connect it to your network with an RJ45 cable (not included) and follow a few simple steps to start controlling your world pharmacy through the internet. As always with Arduino, every element of the platform – hardware, software and documentation – is freely available and open-source. This means you can learn exactly how it's made and use its design as the starting point for your own circuits. Hundreds of thousands of Arduino Boards are already fueling people’s creativity all over the world, every day. 

*Requires an Arduino Board (not included)
•	Operating voltage 5V (supplied from the Arduino Board)
•	Ethernet Controller: W5500 with internal 32K buffer
•	Connection speed: 10/100Mb
•	Connection with Arduino on SPI port
For More Details https://www.arduino.cc/en/Main/ArduinoEthernetShield
