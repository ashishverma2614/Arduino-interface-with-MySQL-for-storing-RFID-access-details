# Arduino-interface-with-MySQL-for-storing-RFID-access-details

Here We are going to connect Arduino UNO, RFID (MFRC522) & Ethernet Shield with MYSQL Database. So for that first we should connect our Arduino Board with the Ethernet Shield & RFID Module.
By using the RFID Module we are going to scan our RFID card and tag which are allow or not. And by using our Ethernet shield we are going to send that data to our MYSQL Database which is connect through a pho page. Bellow we provided the code for PHP as well as for Arduino. You also can go through our video to better understanding how to create a database in MYSQL and how to connect with PHP and Arduino.

See pin Configuration bellow 
NOTE-BECAUSE WE ARE USING TWO SPI DEVICES THAT’S WHY WE HAVE TO CHANGE OUR SS PIN FOR RFID MODULE .
Reader			 Uno	 	 Mega    	  Nano v3   	 Leonardo	 Pro Micro
 * Signal     	 Pin        	  Pin       	    Pin 		      Pin   	     Pin       	       Pin
 * -----------------------------------------------------------------------------------------
 * RST/Reset 	  RST      	    9        		     9      	  	 D9         	RESET/ICSP-5            RST
 * SPI SS      	SDA(SS)    	  4/10       	     4/53    	D10        	10                                  10
 * SPI MOSI   	 MOSI      	   11 / ICSP-4 	     51       	 D11        	ICSP-4          	         16
 * SPI MISO  	  MISO        	 12 / ICSP-1  	     50        	D12       		 ICSP-1                        14
 * SPI SCK  	   SCK         	 13 / ICSP-3 	      52        	D13       		 ICSP-3                15

