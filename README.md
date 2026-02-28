# Train–Worker Smart Alert System Using LoRa

A LoRa-based safety alert system designed to prevent accidents between trains and
railway track maintenance workers by enabling real-time, fail-safe communication.

---

## 🚧 Problem Statement
Railway track maintenance workers operate on active tracks where approaching
trains pose serious safety risks. Due to environmental noise, poor visibility,
and reliance on manual signaling, workers may fail to detect trains in time.
Similarly, train drivers often lack real-time information about worker presence
on the tracks.

---

## 💡 Proposed Solution
This project introduces a smart alert system using **LoRa wireless communication**
between:
- **Pilot Unit (Train Engine)**
- **Worker Safety Unit**

The system uses **presence detection** and **timeout-based fail-safe logic** to
ensure mutual awareness between trains and workers.

---

## 🧠 System Working
- Worker unit sends periodic **heartbeat signals** (`WORKER_PRESENT`)
- Pilot unit listens for worker presence
- If workers are detected → alerts are generated
- If no worker signal is detected → system shows **ALL TRACKS CLEAR**
- Worker unit receives alerts and warns workers using display and LED

---

## 🛠️ Tech Stack
- ESP32 Microcontroller  
- LoRa Module (SX1276 / SX1278)  
- Arduino IDE  
- Embedded C / C++  
- SPI & I2C Communication  
- OLED Display (SSD1306)  
- Breadboard Prototyping  

---

## 📦 Hardware Components
### Pilot (Train) Unit
- ESP32
- LoRa Module
- OLED Display
- USB Power Supply

### Worker Unit
- ESP32
- LoRa Module
- OLED Display
- Red LED
- Breadboard & Jumper Wires

---

## 📂 Repository Structure
