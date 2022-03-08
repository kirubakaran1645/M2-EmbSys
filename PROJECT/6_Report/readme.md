# Introduction

The vehicle having major feature. In this technology it is used to determine the presence of the passanger and if the passanger existing in side the car then our system starts the functionality. So in nowdays everything is becoming automated and everyone is looking for the new products to made the life easier.In our project the main aim is to design and develop the system which is capable of monitoring the passanger's existance and Heat Monitoring and Displaying.
<br>In this, the controller aims at control the temperature in the car. Firstly, if a person is seated in a car then the Button sensor will be activated. If a person is not seated, then the Button sensor will not be activated. When the Button sensor is activated then automatically heater sensor will be activated. Then temperature sensor monitors the temperature and sends analog value to atmega328 microcontroller.

## Features
1.It sense whether the person is existed or not.   
2.The person can request, the Heater accordinging to that the heat will generate.  
3.This system is reliable.  
4.The person can modify the temperature by observing the display which is given in the system.  
5.It is compitable.  

## Used components
 1) Temperature sensor
 2) switches
 3) display
 4) led for indication
 5) potential Switch
 6) resister

 ## SWOT Analysis- Strengths, and Weakness, Opportunities Threats
 ## Strength
 1.Low cost and compitable system.
 <br> 2.User Friendly.
 <br> 3.Easy to modify the temperature values.
 <br> 4.It is efficient and convenient.

 ## Weakness
 1.It can be used only in europian countries.
  <br> 2.Low sensitivity.

## Opportunities
1.It can be implemented by replacing heater by air conditioners.
<br> 2.It will be helpful in all the countries.

## Threats
Because of low senstivity it will not suitable in high temperature Environment.
<br>
<br>
<br>
[![image](https://www.linkpicture.com/q/WhatsApp-Image-2022-03-07-at-21.59.12.jpeg)](https://www.linkpicture.com/view.php?img=LPic622636da01705235870747)

## 4W's and 1'H
## Why
It can monitoring our body temperature even when we are healthy and it can help to detect disease early and help us if it is okay to go to work or college or school.

## What
Seat Monitoring System based on Temperature.

## When
It can be used in only Low temperature.

## Where  
It can be used in Industries like Automobile.

## How
It can be modified by changing the Temperature.
<br>
<br>
[![image](https://www.linkpicture.com/q/WhatsApp-Image-2022-03-07-at-21.59.12-1.jpeg)](https://www.linkpicture.com/view.php?img=LPic622636fb509b0379656239)

## Detail Requirements
## High Level Requirements
| ID | DESCRIPTION | STATUS |
| :--: | :---: | :----: | 
|    1 | Microcontoller | Program for the project |
|    2 | Seat Sensor | Whether the person is existed on seat or not |
|    3 | Temperature Sensor | To measure temperature |
|    4 | Heat Generate | Seat should be heated |
|    5 | Display | Generated heat should be displayed on LCD |

## Low Level Requirements
| ID | DESCRIPTION | STATUS |
| :--: | :---: | :----: |
|         1 | ATmega328 | Here i have used atmega328 microcontroller |
|         2 | PIR(Passive Infrared) sensor | To detect the presence of human |
|         3 | LM355 sensor | To measure temperature |
|         4 | ADC with PWM-Fast | It operate at a wide frequency range |
|         5 | LCD | Temperature should be displayed on LCD |

# Block   Diagram:-

![Block Diagram](https://user-images.githubusercontent.com/70369948/143669285-190349aa-bc30-4a53-bde9-3610c8f6836d.jpg)

# flow chart Diagram:-

![Flow Chart (1)](https://user-images.githubusercontent.com/70369948/143670773-a55fd8a0-f7a7-45a6-8609-2ed61b463506.jpg)

# Activity 1
## Controlling led using button and heater as input 
## In Action

|ON|OFF|
|:--:|:--:|
|![ON](https://user-images.githubusercontent.com/94127613/144220118-c987fb80-cb16-4a37-ba15-3fd00ad5bd00.png)|![OFF](https://user-images.githubusercontent.com/94127613/144220181-c3e33206-0f3f-433c-b704-c708bccfacc7.png)|

# Activity 2
## Reading the temperature from sensor using ADC 

|MAX|RANDOM|
|:--:|:--:|
|![MAX](https://user-images.githubusercontent.com/94127613/144220250-e0e53fa1-3e52-4b11-b12a-8539b3fc74ad.png)|![RANDOM](https://user-images.githubusercontent.com/94127613/144220291-7fffec09-2cf7-4cb4-aff9-cfab931d2fbe.png)|

# Activity 3
## Obtaining PWM signal based on temperature sensor

|PWM 70% duty-cycle|PWM 20% duty-cycle|
|:--:|:--:|
|![PWM_70](https://user-images.githubusercontent.com/94127613/144220391-8d2e218a-4e13-45aa-b12c-8c2550c9f4cd.png)|![PWM_20](https://user-images.githubusercontent.com/94127613/144220446-14117f7a-3e9d-4aa4-be3e-01a641c22a94.png)|

# Activity 4
## Transmitting Temperature value through UART

|Temperature 29 C|Temperature 20 C|
|:--:|:--:|
|![29C](https://user-images.githubusercontent.com/94127613/144220481-4712ccb8-1c50-4bf9-a7ea-40b680115564.png)|![20C](https://user-images.githubusercontent.com/94127613/144220530-24a1cc97-0e0a-4465-b09b-63de3174dec4.png)|

## TEST PLAN and Corresponding Output

### High Level Test Plan


|   Test                                               | Exp I/P                |           Exp O/P            |      Actual Out          |    
| -------------                                        |--------------          | ------                       | ------------------       | 	
| Function of Seat Sensor                              |If person sits on seat  | Detects person               | Detects person           | 	
| Function of Temprature  sensor                       |Temprature change       | Detects Temprature Change    | Detects Temprature Change| 	
| Function of Display                                  |change in heat          | Display the output           | Display the output       | 	
	



### Low Level Test Plan


|   Test                                               | Exp I/P                                     |           Exp O/P            |      Actual Out          |    
| -------------                                        |--------------                               | ------                       | ------------------       | 	
| Temperature changes                                  |if user Temprature=Heater Temprature         | Temprature is displayed      | Temprature is displayed  | 	
| set Heater function                                  |When request sent                            | Sets Heater                  | Sets Heater              | 	








