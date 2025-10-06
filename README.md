# 💧 CSE406 - Lab 01: Real-time Water Level Monitoring using Arduino UNO

## 📘 Objective
To interface a water level sensor with Arduino Uno, read its analog data, convert it into a percentage, and visualize both the water level and its rate of change using the Arduino IDE Serial Plotter.

---

## ⚙️ Hardware & Software Used
- Arduino UNO  
- Water Level Sensor  
- Breadboard & Jumper Wires  
- USB Cable  
- Arduino IDE (for coding and visualization)

---

## 🧩 Circuit Connection
| Sensor Pin | Arduino UNO Pin |
|-------------|----------------|
| S (Signal)  | A0             |
| + (VCC)     | 5V             |
| - (GND)     | GND            |

---

## 💻 Code Features
✅ Reads analog sensor data  
✅ Maps raw data (0–1023) to water level percentage (0–100%) using `map()`  
✅ Prints both raw value and percentage for Serial Plotter visualization  
✅ Displays alerts based on thresholds: LOW, MEDIUM, HIGH  
✅ Calculates rate of change between readings  
✅ Well-commented and beginner-friendly code  

---

## 🔢 Output Threshold Alerts
| Water Level (%) | Alert Message     |
|------------------|------------------|
| 0–25%            | VERY LOW LEVEL   |
| 25–75%           | LOW LEVEL        |
| 75–95%           | MEDIUM LEVEL     |
| 95–100%          | HIGH LEVEL       |

---

## 📊 Example Output
Water Level: 78.23%
Rate of Change: 2.45%
MEDIUM LEVEL

---

## 🧠 Learning Outcome
- Understand analog sensor data acquisition  
- Learn data mapping and percentage scaling  
- Implement conditional alerts based on thresholds  
- Visualize dynamic data using Arduino Serial Plotter  
- Apply simple IoT-style data monitoring logic  

---

## 👨‍💻 Author
**Saifur Rahman**  
Department of Computer Science and Engineering  
East West University  
Spring 2025 | Course: CSE406 (Internet of Things)  
Instructor: *Dr. Raihan Ul Islam*

---

### 🗂️ GitHub Folder Structure
CSE406-Internet-of-Things-Labs/
└── Lab01_WaterLevelSensor/
├── Lab01_WaterLevelSensor.ino
└── README.md
