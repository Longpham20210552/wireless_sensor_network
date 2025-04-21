
**🔌 Project: Wireless Sensor Network for Temperature & Humidity Monitoring**

This project implements a wireless sensor network to measure and collect temperature and humidity data from multiple sensor nodes. The data is transmitted via RF communication to a central gateway connected to a computer or server for real-time monitoring and data management. This system is designed for smart agriculture and environmental monitoring applications.

![image](https://github.com/user-attachments/assets/5e240463-9d48-4f6a-ac58-f94116c29507)


**Gateway**_(Gateway folder)_: Managing communication with multiple sensor nodes via RF. Scheduling and collecting temperature/humidity data from nodes. Sending collected data to a web server via HTTP. Receiving configuration commands from the server.

**Sensor Node**_(SensorNode folder)_ : Measuring temperature and humidity using environmental sensors (e.g., DHT22/SHT20). Take the control commands from and sending data to gateway. Supporting LED alerts based on configurable threholds.

## ⚙️ Hardware Used

- ESP32 Wroom 
- STM32F103C8T6 ("Blue Pill")
- LoRa modules (SX1278)
- SHT21 sensors
- LEDs, battery pack

## 🔁 Data Flow

1. Gateway sends broadcast signal.
2. Each node sends back its sensor data.
3. Gateway uploads all data to the server via HTTP.
4. Server displays or logs the data.

## 📊 Project Achievements

- ✅ Accuracy: < 1°C, Resolution: 0.1°C
- ✅ 11 nodes support (tested with 4 nodes)
- ✅ Update interval: <10 seconds
- ✅ Battery runtime: 8+ hours
- ✅ Web-based data visualization
