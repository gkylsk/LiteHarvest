# lite_harvest

LITE HARVEST: Wick-Based Hydroponics System With Mobile  Application
This project focuses on the development of a wick-based hydroponics system integrated with sensors and a mobile application for remote monitoring and control. The objectives were to design a hardware setup capable of monitoring temperature, TDS, and EC levels in water, automate water flow control, and provide real-time data visualization and notifications through a mobile app.  The hardware comprises temperature, and TDS sensors placed in water bucket which is connected to a water motor controlling water flow to cups of plant in the hydroponic setup. A water level sensor ensures optimal water levels. Data from the sensors are transmitted to a cloud database via Wi-Fi. The mobile application enables users to access setup instructions, view real-time temperature, TDS, and EC values, and receive notifications if thresholds are exceeded. Admins have additional privileges to manage user accounts. In the findings, the hardware successfully measures and controls environmental parameters, ensuring optimal growing conditions for the plants. The mobile application provides intuitive user interface and effective data visualization, enhancing user experience and facilitating remote monitoring. Threshold notifications enable timely intervention, contributing to improved plant health and yield.

<img src="![alt text](image.png)" alt="Hardware-1" width="250" height="300">
<img src="![alt text](image-1.png)" alt="Hardware-2" width="250" height="300">
<img src="![alt text](image-2.png)" alt="Wick setup" width="350" height="200">
<img src="![alt text](image-3.png)" alt="Home Page" width="200" height="400">
<img src="![alt text](image-4.png)" alt="Admin Dashboard" width="200" height="400">
<img src="![alt text](image-5.png)" alt="Management Login" width="200" height="400">
<img src="![alt text](image-6.png)" alt="Dashboard" width="200" height="400">
<img src="![alt text](image-7.png)" alt="Notification" width="200" height="400">

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
