# group-07 ![CI App](https://github.com/DIT112-V20/group-07/workflows/CI%20App/badge.svg) ![CI Arduino](https://github.com/DIT112-V20/group-07/workflows/CI%20Arduino/badge.svg)

![TeamLogo](https://cdn.discordapp.com/attachments/713314260222214226/714407241121398794/007.png)

## Demo Video
- [Project 007 Demo Video](https://www.youtube.com/watch?v=PAH5nVPPHcs)

## Project
### WHAT?
This project works towards an automated last-mile delivery service. The vision is that an autonomous driving car delivers packages to a specified address. On top the end-user could see the driving process and ETA in a mobile application.\
At this stage of development the car drives not fully autonomous, it still needs a human driver controlling the car with an android app. But, if the car detects an obstacle in front it is able to drive around it without input from the driver.\
On the apps side, end users are able to select a delivery address on a map, and a driver can then see that address on a map in combination with a route towards the drop off location. 

### WHY?
To make it easier for customers to get deliveries, since an autonomous delivery system does not have the constraints that a system using a human driver has, so deliveries can be made whenever the customer desires. Also making delivery of expensive goods  safer since, during transport, no human interaction will be necessary other than that of the customer.

### HOW?
We plan on using the following technologies to complete this project: 
- the Arduino IDE and the Smart Car Shield library to control the car
- Sensors to be able to detect obstacles in the car’s path
- Something similar to the GPRS+GPS Quadband Module for Arduino to track the localisation of the car
- Android studio or something similar to create the application that is able to track the localisation of the car.

## Resources
To read more about the Smartcar, please see the documentation provided by [@platisd](https://github.com/platisd): [_'Smartcar gets an ESP32 upgrade'_](https://platis.solutions/blog/2020/02/16/smartcar-gets-an-esp32-upgrade/)
### Hardware
- 1x Smartcar
- 2x Ultrasonic Sensor
- 1x Micro Lidar Sensor
- 2x Breadboard
- 1x Neo GPS 6m Module
- 1x Android Smartphone

### Software
- Arduino IDE
- Android Studio
- Smartcar Library
- Bluetooth Serial Library
- VL53L0X Library
- Wire Library
- [TinyGPSPlus](https://github.com/mikalhart/TinyGPSPlus) library

## Setup

### Smartcar
To set-up the car, please see the documentation provided by [@platisd](https://github.com/platisd): [_'Smartcar Library'_](https://github.com/platisd/smartcar_shield)
#### Sensors
- Attach one Ultrasonic Sensor to the front of the car, connect the trig pin to D19 & the echo pin to D5
- Attach one Ultrasonic Sensor to the right side of the car, connect the trig pin to D33 & the echo pin to D18
- Attach one Micro Lidar Sensor directly to the left side of the car
- Attach the GPS module to the car and connect the GPS RXPin to D16 and the TXPin to D17

#### Calibration
To calibrate the car, please see the documentation provided by [@platisd](https://github.com/platisd): [_'Smartcar Library'_](https://github.com/platisd/smartcar_shield)

Sensors that need to be calibrated: 
- Gyroscope 
- Odometer
- Ultrasonic Sensors
- Micro Lidar Sensro

Methods that need calibration:
- STEERING_OFFSET_FORWARD
- STEERING_OFFSET_BAKWARDS

#### Software
- Go to the Arduino IDE's library manager and install the following libraries:
    - Smartcar shield
    - VL53L0X
- Dowlonad the [TinyGPSPlus](https://github.com/mikalhart/TinyGPSPlus) library and include it to Arduino's library folder
- Set the Board in the Arduino IDE to DOIT ESP32 DEVKIT 1
- Compile and upload the code to the car

### App
- Google play services SDK
- Enable USB debugging on your android phone and connect it via USB to your computer to be able to download the application.

### User Manual
![Selection](https://i.imgur.com/zAEGNVP.jpg)
- This is where you can choose to either be a driver or a user.
- By pushing the "DRIVER"-button you will be able to control the car by using the controls displayed below.
- By pushing the "USER"- button it will send you to the User's screen which is the map.

![Controller](https://i.imgur.com/8RqL9Vr.jpg)
- You can connect to the car by using the "CONNECT TO BLUETOOTH"-button.
- By pressing the "START"-button you will make the car drive forward in gear 1.
- By pressing the "STOP"-button the car will stop.
- If you want the car to go in reverse, you press the "Reverse"-button.
- To control the car's speed and steering use the two sliders on the screen.
- To open the map, click the "MAP"-button.

![User](https://i.imgur.com/nykkonX.jpg)
- Here you can see the car's location which is displayed by a green marker.
- You can set the destination by either pressing on the map or entering the desired address on the search bar.
- A path will automatically appear on the map between the car and the desired location.

## Developers
- [Oscar Hjern](https://github.com/oscarhjern), SCRUM Master 
- [Maja Wennroth](https://github.com/majawennroth), Responsible of Car    
- [Mikael Höije](https://github.com/mikaelhoije), App Guy 
- [Jakob Sixten](https://github.com/sijakob), Connection Specialist 
- [Johann Tammen](https://github.com/johann-tam), Git Master 
- [Maximilien Uddgren](https://github.com/WhiteMaken), App Guy 

## Contact 
To contact the team with questions regarding the 007-project, please create an issue and a team member will assist you with your inquiry. To contact the team regarding questions of the Smartcar platform, please direct your questions towards [@platisd](https://github.com/platisd). To come in contact with individual team members we have linked their profiles on this page. The rest is up to you, good luck! 
