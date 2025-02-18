# Embedded-System
EE3427 class
# Smart-Home-Security-System-using-STM32
## Functional-Requirements
1.  Intrusion Detection: The system shall detect motion using PIR sensors and unauthorized entry via magnetic door/window sensors.
2.	Flam Detection: The system shall detect when a fire or flame occurs.
3.	Alarm Activation: The system shall trigger a buzzer alarm upon detecting unauthorized entry.
4.	Alert Notifications: The system shall send real-time SMS notifications via GSM and/or mobile app alerts via Wi-Fi when an intrusion is detected.
5.	Remote Arm/Disarm: The system shall allow users to enable or disable security remotely via a mobile app or SMS command.
6.	Real-time Display: The system shall display the security status and sensor activity on an OLED screen.
7.	Camera Capture (Optional): The system shall capture an image of the intruder using an OV7670 camera module and store/send it to a cloud server.
8.	Power Backup Support: The system shall include a battery backup to remain operational during power failures.
## Non-Functional-Requirements
1.	Real-time Processing: The system shall process sensor data and respond within 500 milliseconds.
2.	Power Efficiency: The system shall operate in low-power mode when idle to conserve energy.
3.	Security & Encryption: The system shall use AES encryption for secure communication with the mobile app/cloud.
4.	Scalability: The system shall support additional sensors, cameras, and cloud-based features for future enhancements.
5.	Reliability & Uptime: The system shall maintain at least 99.5% uptime, ensuring continuous security monitoring.
# Components
| **Component** | **Specification** |
| --- | --- |
| Microcontroller | STM32F103RCT6 |
| PIR Motion Sensor | HC-SR501 |
| Flame Sensor | IR Flame Sensor Module (HS0242) |
| Magnetic Door/Window Sensor | Detects forced entry |
| Buzzer | Sounds alarm |
| OLED Display | Shows security status (0.96” I2C) |
| Camera Module (Optional) | Captures images on intrusion (OV7670) |
| Wi-Fi Module | Sends alerts to a mobile app (ESP8266/ESP32) |
| GSM Module (Optional) | Sends SMS alerts (SIM800L) |
| Relay Module | Controls lights or locks |
| Battery Backup | Ensures security during power cuts |
# Block-Diagram
![Image](https://github.com/user-attachments/assets/5dde3028-7999-4c93-9234-fc501d587500)
