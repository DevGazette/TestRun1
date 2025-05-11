# Air Quality Control System
This project involves the design and development of a sensor-based system to monitor and analyze air quality in a basement environment. The system aims to detect pollutants and ensure a healthy indoor atmosphere.

## 🛠️ Technologies Used
Sensors: MQ-135 gas sensor for detecting harmful gases such as ammonia (NH₃), nitrogen oxides (NOₓ), benzene, smoke, and carbon dioxide (CO₂).

Microcontroller: Arduino Uno for interfacing with sensors and processing data.

Data Transmission: ESP8266 Wi-Fi module to transmit collected data to a cloud-based platform.

Cloud Platform: ThingSpeak for real-time data visualization and analysis.

Programming Languages: Firmware developed using C++ for Arduino; MATLAB used for data analysis on the cloud platform.

## 🔑 Key Features
Real-Time Monitoring: Continuous monitoring of air quality parameters, including concentrations of various gases and particulate matter.

Data Logging: Historical data storage to analyze trends and identify potential pollution sources.

Alerts: Threshold-based alerts to notify users when pollutant levels exceed safe limits.

User Interface: User-friendly dashboard for visualizing air quality metrics and system status.

## ⚙️ Challenges and Solutions
Sensor Calibration: Ensured accurate readings by calibrating sensors against known concentration standards.

Environmental Factors: Accounted for temperature and humidity variations by incorporating DHT22 sensors and adjusting readings accordingly.

Data Accuracy: Implemented data smoothing algorithms to filter out noise and improve the reliability of readings.

## 📡 System Architecture
The system architecture comprises the following components:

MQ-135 Gas Sensor: Detects various harmful gases and outputs analog signals corresponding to gas concentrations.

DHT22 Sensor: Measures ambient temperature and humidity to provide environmental context for gas readings.

Arduino Uno: Processes sensor data and communicates with the ESP8266 module.

ESP8266 Wi-Fi Module: Transmits processed data to the ThingSpeak cloud platform over Wi-Fi.

ThingSpeak Cloud Platform: Stores and visualizes real-time and historical air quality data, enabling remote monitoring and analysis.

## 📈 Getting Started
To set up and run the Air Quality Control System:

Hardware Setup:

Connect the MQ-135 sensor to the Arduino Uno's analog input.

Connect the DHT22 sensor to a digital input on the Arduino.

Connect the ESP8266 module to the Arduino for Wi-Fi communication.

Software Setup:

Install the Arduino IDE and required libraries for the MQ-135 and DHT22 sensors.

Upload the firmware from the src/ directory to the Arduino Uno.

Configure the ESP8266 module with your Wi-Fi credentials and ThingSpeak API key.

Cloud Configuration:

Set up a ThingSpeak channel with fields corresponding to the sensor data (e.g., gas concentration, temperature, humidity).

Use MATLAB scripts on ThingSpeak for advanced data analysis and visualization.
