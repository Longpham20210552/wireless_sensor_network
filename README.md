
**🔌 Project: Wireless Sensor Network for Temperature & Humidity Monitoring**

This project implements a wireless sensor network to measure and collect temperature and humidity data from multiple sensor nodes. The data is transmitted via RF communication to a central gateway connected to a computer or server for real-time monitoring and data management. This system is designed for smart agriculture and environmental monitoring applications.

![image](https://github.com/user-attachments/assets/5e240463-9d48-4f6a-ac58-f94116c29507)


**Gateway**_(Gateway folder)_: Managing communication with multiple sensor nodes via RF. Scheduling and collecting temperature/humidity data from nodes. Sending collected data to a web server via HTTP. Receiving configuration commands from the server.

**Sensor Node**_(SensorNode folder)_ : Measuring temperature and humidity using environmental sensors (e.g., DHT22/SHT20). Take the control commands from and sending data to gateway. Supporting LED alerts based on configurable threholds.
