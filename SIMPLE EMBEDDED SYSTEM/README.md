# SIMPLE EMBEDDED SYSTEM



   ## LPG GAS LEAKAGE DETECTION 



### OBJECTIVE:


1) Detect Gas Leakage (like LPG leak, Butane leak,
Methane leak) or any such petroleum based gaseous substance that can be detected
using MQ5 Sensor.

2) Produce a sound alarm upon gas leak and stop the
alarm once gas leak is under control (gas presence in atmosphere is under
normal range)
       
3) Display status in an LCD using a 16×2 LCD module.



## REQUIREMENTS:



  ### HIGHLEVEL REQUIREMENTS




1) Arduino should able to detect the LPG leakage whenever the gas gets
leaked. 



2) Arduino should able to alert the user when the gas gats leaked.



3) Arduino should able to show the alert message.



                                        
 ### LOWLEVEL REQUIREMENTS



1) Ardunio should able to detect the LPG leakage detection using MQ2
sensor.



2) Arduino should able to alert the user with Buzzer and LED. 



3) Arduino should able to show alert message using LCD display.



## BLOCK DIAGRAM:
![Screenshot (41)](https://user-images.githubusercontent.com/98970879/154853372-4eaa1100-4fa7-47fc-aad2-0c7e94ea639f.png)







 
  
 
 
  
  
 



 

 






                                           



               








 
  
  
  
  
  
  
  
  
 
 
  
  
  
 
 
  
  
 
 
  
 
 
  
 
 
  
  
  
 
 
  
  
  
 
 
  
 



 

 






## COMPONENT USED:



1) Arduino Uno



2) MQ-2 sensor



3) Buzzer

4)   16x2 LCD


5) 1K resistor



6) Bread board



7) 9 volt battery


8) Connecting wires



 



## Arduino uno:



 Arduino Uno is a microcontroller board based on the ATmega328P . It has 14 digital input/output pins (of which 6 can be used as
PWM outputs), 6 analog inputs, a 16 MHz ceramic resonator , a USB connection, a power jack, an ICSP header and a reset button.




 
  
  Microcontroller - ATmega328P


  Operating Voltage - 5V

Input Voltage (recommended) - 7-12V


  
 
 
  
 Input Voltage (limit) - 6-20V


  
 
 
  
  Digital I/O Pins - 14 (of which 6 provide PWM
  output)


  
 
 
  
  ## MQ-2 Gas sensor:


  
  
   


  
 
 
  
   


  
  
   


  
 
 
  
  MQ2 is
  one of the commonly used gas sensors in MQ sensor series. It is a Metal Oxide
  Semiconductor (MOS) type Gas Sensor also known as Chemiresistors as
  the detection is based upon change of resistance of the sensing material when
  the Gas comes in contact with the material. Using a simple voltage divider
  network, concentrations of gas can be detected.MQ2 Gas sensor works on 5V DC
  and draws around 800mW. It can detect LPG, Smoke, Alcohol,
  Propane, Hydrogen, Methane and Carbon Monoxide concentrations
  anywhere from 200 to 10000ppm.


 ## Buzzer:


  A
  buzzer or beeper is an audio signalling device, which may be
  mechanical, electromechanical, or piezoelectric (piezo for short). ...
  Typical uses of buzzers and beepers include alarm devices, timers, and
  confirmation of user input such as a mouse click or keystroke.


 ##  LCD Display:


  A
  liquid-crystal display (LCD) is a flat-panel display or other
  electronically modulated optical device that uses the light-modulating
  properties of liquid crystals combined with polarizers. Liquid crystals
  do not emit light directly, instead using a backlight or reflector to produce
  images in color or monochrome.


 ## Bread Board:


  A breadboard is used to make up temporary
  circuits for testing or to try out an idea. No soldering is required
  so it is easy to change connections and replace components. Parts are not
  damaged and can be re-used afterwards.


 ## WORKING:


  The functioning of the circuit is very simple. Once the device is powered ON, the Arduino initializes the LCD
  display and start reading the analog voltage from the MQ-2 sensor. The analog voltage from the sensor is digitized using the in-built ADC channel and
  stored in a variable as a 10-bit value. The sensor value is compared with a calibrated threshold and if the sensor value exceeds that value, the buzzer
  is activated and a RED light LED will ON . If the sensor value remains within limits, a message showing “No Danger” keeps on displaying on the LCD screen
  and the GREEN light LED will ON. The buzzer is kept OFF for the condition.


  

  ## Conclusion:


  

  After this project performance, can conclude that detection of the LPG gas leakage is incredible
  in the project system. Applicable usefully in the industrial and domestic purpose.
  In danger situations we are able to save the life by using this system. A sensor node senses gas like CO2, oxygen,
  propane. The estimated range of transmission and consumption of power is obtained. The simple procedures and Arduino UNO Micro controller area used to
  build the sensor.


   


   


   


  
  
   


  
 

