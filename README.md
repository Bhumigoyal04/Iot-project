# Iot-project
IoT Smart Exhaust Fan with RFID, Gas, Flame, and Environmental Monitoring
This project involves building a smart exhaust fan system controlled via Blynk, an IoT platform. The system is equipped with various sensors to monitor environmental conditions such as temperature, humidity, gas levels, and flame detection. It also includes an RFID access control mechanism for user authentication.

Features:
Blynk Integration: Allows for remote control and monitoring of the exhaust fan system via the Blynk mobile app.

RFID Authentication: Users can unlock the system using an RFID card with a valid UID. Unauthorized access triggers an alarm.

Environmental Monitoring: The system reads temperature, humidity, and gas levels from the DHT11 and MQ2 sensors, displaying the data on an LCD screen and updating the Blynk app.

Automatic Fan Control: The fan automatically activates when gas levels exceed a certain threshold (40%), or can be manually controlled via the Blynk app.

Flame Detection: A flame sensor detects fire hazards, and its status is displayed on the LCD and updated on Blynk.

Servo-Controlled Gate: A servo motor controls the gate opening/closing based on RFID authentication, allowing secure access to the system.

Hardware:
ESP32: Microcontroller to manage all sensors and connect to Blynk.

RFID Reader (MFRC522): Used to scan RFID cards for user authentication.

MQ2 Gas Sensor: Detects gas levels and provides real-time monitoring of air quality.

DHT11 Temperature & Humidity Sensor: Provides temperature and humidity data.

Flame Sensor: Detects flames or fire in the environment.

Servo Motor: Controls the gate for secure access.

LCD (I2C): Displays real-time sensor data and system status.

Buzzer: Alerts the user for unauthorized access or system status changes.

Components:
ESP32 Microcontroller

RFID MFRC522 Module

DHT11 Temperature & Humidity Sensor

MQ2 Gas Sensor

Flame Sensor

Servo Motor

LCD Display (I2C)

Buzzer

Relay Module (for fan control)

Setup:
Connect all the components according to the provided pin definitions in the code.

Configure the Blynk app with your credentials and corresponding virtual pins.

Upload the code to your ESP32 and run the system.

Usage:
Scan an RFID card to access the system. If the UID matches the valid ID, the servo motor will rotate, and access will be granted.

The exhaust fan automatically activates when the gas levels exceed 40%, or you can manually control the fan using the Blynk app.

The system continuously monitors and displays environmental data (temperature, humidity, gas levels, flame detection) on the LCD and in the Blynk app.

