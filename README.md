# Arduino-interface-with-MySQL-for-storing-RFID-access-details

Here We are going to connect Arduino UNO, RFID (MFRC522) & Ethernet Shield with MYSQL Database. So for that first we should connect our Arduino Board with the Ethernet Shield & RFID Module.
By using the RFID Module we are going to scan our RFID card and tag which are allow or not. And by using our Ethernet shield we are going to send that data to our MYSQL Database which is connect through a pho page. Bellow we provided the code for PHP as well as for Arduino. You also can go through our video to better understanding how to create a database in MYSQL and how to connect with PHP and Arduino.

See pin Configuration bellow 
NOTE-BECAUSE WE ARE USING TWO SPI DEVICES THAT’S WHY WE HAVE TO CHANGE OUR SS PIN FOR RFID MODULE .

.. _pin layout:
Pin Layout
----------

The following table shows the typical pin layout used:

+-----------+----------+---------------------------------------------------------------+--------------------------+
|           | PCD      | Arduino                                                       | Teensy                   |
|           +----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
|           | MFRC522  | Uno / 101   | Mega    | Nano v3 |Leonardo / Micro | Pro Micro | 2.0    | ++ 2.0 | 3.1    |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
| Signal    | Pin      | Pin         | Pin     | Pin     | Pin             | Pin       | Pin    | Pin    | Pin    |
+===========+==========+=============+=========+=========+=================+===========+========+========+========+
| RST/Reset | RST      | 9 [1]_      | 5 [1]_  | D9      | RESET / ICSP-5  | RST       | 7      | 4      | 9      |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
| SPI SS    | SDA [3]_ | 10 [2]_     | 53 [2]_ | D10     | 10              | 10        | 0      | 20     | 10     |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
| SPI MOSI  | MOSI     | 11 / ICSP-4 | 51      | D11     | ICSP-4          | 16        | 2      | 22     | 11     |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
| SPI MISO  | MISO     | 12 / ICSP-1 | 50      | D12     | ICSP-1          | 14        | 3      | 23     | 12     |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+
| SPI SCK   | SCK      | 13 / ICSP-3 | 52      | D13     | ICSP-3          | 15        | 1      | 21     | 13     |
+-----------+----------+-------------+---------+---------+-----------------+-----------+--------+--------+--------+

.. [1] Configurable, typically defined as RST_PIN in sketch/program.
.. [2] Configurable, typically defined as SS_PIN in sketch/program.
.. [3] The SDA pin might be labeled SS on some/older MFRC522 boards. 
