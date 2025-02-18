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
## Requirement
| **Component** | **Specification** | **Reason** |
| --- | --- | --- |
| Microcontroller | STM32F103RCT6 | easy to use, many GPIO, USB to UART, LED, Buttons, Medium price, 5V |
| PIR Motion Sensor | Motion detection using changes in infrared radiation | cheap, easy to use, low power |
| Flame Sensor | Flame detection | cheap, easy to use |
| Magnetic Door/Window Sensor | Detects forced entry | cheap, easy to use, low power |
| Buzzer | Sounds alarm | cheap, easy to use, low power |
| OLED Display (0.96” I2C) | Shows security status | cheap, easy to use, low power |
| Camera Module (OV7670, Optional) | Captures images on intrusion | cheap, easy to use, low power |
| Wi-Fi Module (ESP8266/ESP32) | Sends alerts to a mobile app | cheap compare to other module, UART, low power |
| GSM Module (SIM800L, Optional) | Sends SMS alerts | Optional might add in the process |
| Relay Module | Controls lights and locks | 4 relay for 2 doors and 2 lights |
| Battery Backup | Ensures security during power cuts | to secure power efficiency |
## Expected
![Image](https://github.com/user-attachments/assets/8d9068e5-2a75-4f72-8b49-2fd3407e9df2)
![Image](https://github.com/user-attachments/assets/9446df2c-f4c6-4857-bb5d-66dc713f8c78)
# Block-Diagram
![Image](https://github.com/user-attachments/assets/5dde3028-7999-4c93-9234-fc501d587500)
