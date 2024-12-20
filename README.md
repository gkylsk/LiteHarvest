# lite_harvest

LITE HARVEST: Wick-Based Hydroponics System With Mobile  Application
This project focuses on the development of a wick-based hydroponics system integrated with sensors and a mobile application for remote monitoring and control. The objectives were to design a hardware setup capable of monitoring temperature, TDS, and EC levels in water, automate water flow control, and provide real-time data visualization and notifications through a mobile app.  The hardware comprises temperature, and TDS sensors placed in water bucket which is connected to a water motor controlling water flow to cups of plant in the hydroponic setup. A water level sensor ensures optimal water levels. Data from the sensors are transmitted to a cloud database via Wi-Fi. The mobile application enables users to access setup instructions, view real-time temperature, TDS, and EC values, and receive notifications if thresholds are exceeded. Admins have additional privileges to manage user accounts. In the findings, the hardware successfully measures and controls environmental parameters, ensuring optimal growing conditions for the plants. The mobile application provides intuitive user interface and effective data visualization, enhancing user experience and facilitating remote monitoring. Threshold notifications enable timely intervention, contributing to improved plant health and yield.

<img src="https://github.com/user-attachments/assets/4091f423-026a-4dad-8a64-4355274ec6b8" alt="Hardware-1" width="250" height="300">
<img src="https://github.com/user-attachments/assets/2a9f9e41-19ae-4ace-acfd-f5d15525de0b" alt="Hardware-2" width="250" height="300">
<img src="https://github.com/user-attachments/assets/4957a689-5606-4a62-9fcd-f9da867d541f" alt="Wick setup" width="350" height="200">
<img src="https://github.com/user-attachments/assets/e69b5c7f-9aa6-4f84-854f-175fdc68ad42" alt="Home Page" width="200" height="400">
<img src="https://github.com/user-attachments/assets/8cab1071-b09e-4524-a8df-edda1b609997" alt="Admin Dashboard" width="200" height="400">
<img src="https://github.com/user-attachments/assets/c037960a-a461-4bfa-9252-5c3a07fa5f53" alt="Management Login" width="200" height="400">
<img src="https://github.com/user-attachments/assets/03f16e41-76bd-403f-ad77-f1a1b8c1c09c" alt="Dashboard" width="200" height="400">
<img src="https://github.com/user-attachments/assets/84922078-210d-4d09-8754-70b4bddfa9bb" alt="Notification" width="200" height="400">

## Download App in Phone 
The system and mobile should be connected to the same network
### Wireless debugging 
Go to phone settings

Select on version

Click Build number until developer options are enabled

Go to developer options 

On wireless debugging

Run the following code in the terminal using path cd C:\Users\Admin\AppData\Local\Android\Sdk\platform-tools 

>./adb tcpip 5555

>./adb connect [IP address]

or

>.\adb pair [IP address]:[Paring code]

Go back to the project file and run the code

## Database
Used Firebase for real-time database

To be able to obtain real-time data the Firebase project fingerprint needs to be uploaded to FirebaseHttpClient.h file

## Notifiction
Download simple push app

Upload code to ESP8266 by providing the key
