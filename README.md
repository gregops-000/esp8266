# esp8266
🚀 #ESP8266 #IoT #OpenSource

This project uses an **ESP8266-based Wemos D1 Mini** board to monitor an **IR barrier sensor** and send real-time **WhatsApp alerts** when the beam is interrupted. A built-in **web interface** provides a live count of detected events and timestamps.

---

## 📸 Project Overview

- IR sensor detects object crossing the beam.
- ESP8266 sends a WhatsApp alert using [CallMeBot API](https://www.callmebot.com/).
- Simple HTTP web server displays count and last event time.
- Uses NTP for accurate timestamps (with timezone offset).
- Ideal for gateways, pets, automation, or security applications.

---

## ✨ Features

- 📶 Wi-Fi connectivity  
- 🧠 IR sensor state monitoring (D1 / GPIO5)  
- 💬 WhatsApp alerts on beam interruption  
- 🌐 Web page for live monitoring  
- 🕒 NTP time with fixed offset for Poland (UTC+2)  
- 💾 Lightweight footprint on ESP8266  

---

## 🧰 Hardware Required

| Component           | Description                        |
|--------------------|------------------------------------|
| Wemos D1 Mini       | ESP8266-based microcontroller      |
| IR Barrier Sensor   | Digital output (beam break sensor) |
| Micro USB Cable     | For power and programming          |
| Internet Access     | For WhatsApp and NTP               |

---

## 🔌 Wiring

<img width="450" height="434" alt="image" src="https://github.com/user-attachments/assets/24552aff-6916-419e-823c-3493dba82e30" />

IR Sensor OUT → D1 (GPIO2)
VCC → 3.3V
GND → GND

📦 Libraries Used
Install via Arduino Library Manager:

- 🌐 ESP8266WiFi

- 🌐 ESP8266HTTPClient

- 🌐 ESP8266WebServer

- 🌐 NTPClient

- 🌐 WiFiUdp

- 🌐 UrlEncode by Masayuki Sugahara

🚀 Getting Started
Clone or download this repository.
file: esp8266-Tokio-IR-Barrier

Replace Wi-Fi and CallMeBot credentials:
    const char* ssid = "YOUR_WIFI_SSID";
    const char* password = "YOUR_WIFI_PASSWORD";
Select board: LOLIN(WEMOS) D1 R2 & mini
Open Serial Monitor at 115200 baud.
Upload to your board/ file: esp8266-Tokio-IR-Barrier

Access the web interface and test alerts.

🧪 Example Serial Output:

WiFi connected. IP: 192.168.2.219
Web server started.
🔴 Barrier Broken! Sending WhatsApp...
✅ WhatsApp message sent
🟢 Barrier Clear.


📜 License

MIT License

Feel free to use, modify, and share this project.