🌡️💧 CSE406 - Lab 02: Temperature, Humidity & Water Level Monitoring using Arduino UNO and ESP8266
📘 Objective

To design and implement a real-time monitoring system that measures temperature, humidity, and water level using DHT11 and Water Level Sensor, with ESP8266 enabling Wi-Fi connectivity for future IoT integration.
⚙️ Hardware & Software Used

Arduino UNO

DHT11 Temperature & Humidity Sensor

Water Level Sensor

ESP8266 Wi-Fi Module

Breadboard & Jumper Wires

Arduino IDE
🧩 Circuit Connections
| Component          | Arduino Pin                  | Description                   |
| ------------------ | ---------------------------- | ----------------------------- |
| DHT11 Signal       | D4                           | Sensor data line (GPIO2)      |
| Water Level Sensor | A0                           | Analog water level input      |
| ESP8266 TX         | D3                           | Serial RX input to Arduino    |
| ESP8266 RX         | D4 (through voltage divider) | Serial TX output from Arduino |
| GND                | GND                          | Common ground                 |
| VCC                | 3.3V / 5V                    | Power supply                  |


💻 Code Features

✅ Reads temperature and humidity using DHT11
✅ Reads water level via analog sensor
✅ Converts raw sensor data into meaningful percentages
✅ Displays all sensor readings on Serial Monitor
✅ Uses calibration constants to accurately map dry/wet readings
✅ Code structured for easy extension to Wi-Fi or cloud-based IoT

🧠 Working Principle

The DHT11 sensor measures air temperature and humidity.

The water sensor outputs an analog signal based on water contact level.

These values are processed by Arduino, scaled to percentages, and displayed via Serial Monitor.

The ESP8266 module allows future Wi-Fi connectivity for IoT data upload.

🔢 Output Example
Temp: 29.4 °C   Hum: 56.8 %   WaterRaw: 715   Water~: 77 %


🧪 Calibration Notes

Adjust the following constants to match your specific sensor:
const int DRY_RAW = 150;   // Reading when sensor is dry
const int WET_RAW = 900;   // Reading when sensor is submerged
Changing these values improves accuracy for your setup.
📊 Example Serial Plotter Visualization

You can visualize dynamic temperature, humidity, and water-level trends using Arduino’s Serial Plotter tool in real time.

🧠 Learning Outcomes

Interface multiple analog/digital sensors with Arduino

Process and calibrate real-time environmental data

Apply data mapping techniques for percentage scaling

Understand ESP8266’s role in IoT systems

Gain experience in structured, modular Arduino programming


👨‍💻 Author

Saifur Rahman
Department of Computer Science and Engineering
East West University
Spring 2025 | Course: CSE406 (Internet of Things)
Instructor: Dr. Raihan Ul Islam
