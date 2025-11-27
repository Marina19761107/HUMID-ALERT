# HUMID-ALERT
The proposed project is an Automated Humidity Alert System designed to monitor indoor humidity and temperature levels using a Raspberry Pi equipped with a Sense HAT. The system helps maintain a stable home environment by notifying the user when humidity exceeds a defined threshold (50%). This allows timely manual activation of a humidifier or heating system to regulate comfort and air quality.

Advanced: To evaluate system performance, humidity data will be collected over one week and analyzed by time of day. The analysis results will provide insights into daily humidity patterns and help anticipate when to switch on the humidifier or heating system during the day.

Tools, Technologies and equipment
Hardware: Raspberry Pi (central controller for processing and networking), Sense HAT (reads humidity and temperature).
Connectivity: Wi-Fi connection for sending data to the cloud.
Programming Language: Python (used for sensor logic and data handling).
IoT Platform: Blynk Cloud (used for mobile dashboard, cloud storage, device management, and notifications).
Protocols: MQTT (for efficient IoT communication).
System workflow:
1.	Sense HAT reads humidity and temperature.
2.	Raspberry Pi sends data to Blynk.
2.1.	Formats the reading into JSON
3.	Data is transferred to the Blynk Cloud using MQTT/HTTP protocols. 
4.	Blynk dashboard shows: Humidity level, Temperature and Alert status.
5.	Blynk triggers notification:
If humidity.50% “Switch on humidifier”
If humidity <50% - “Humidity is normal”
6.	Data is stored in the Blynk cloud for visualization and history tracking.
7.	Data analysis: 
6.1. Humidity readings are collected over a week.
6.2. Values are grouped by time of day (morning, afternoon, evening).
6.3. Average humidity patterns are identified.
6.4. Insights help anticipate when humidity is usually higher and optimize when to switch on the humidifier or heating system.

Project Repository:
A project repository has been created to store all files, code, and documentation. 
https://github.com/Marina19761107/HUMID-ALERT/edit/main/README.md
