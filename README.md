# ESP Weather Station

An ESP32-based weather station project developed as a university assignment.

## Architecture

```text
ESP32
├── Sensors
│   ├── DS18B20 - Front temperature
│   └── DS18B20 - Back temperature
│
├── OLED Display
├── Wi-Fi
│
├── Web Server
│   ├── Web Dashboard
│   │   ├── Front & back temperature + weather conditions
│   │   ├── 7-day weather forecast
│   │   ├── FoxESS solar panel statistics
│   │   └── ZKM Gdynia bus departures
│   │
│   ├── REST API
│   └── WebSocket - live sensor updates
│
├── Weather API
├── FoxESS API
└── ZKM Gdynia API
```

## Core Features

- Real-time temperature measurements from two DS18B20 sensors
- Temperature and weather information displayed on an OLED screen
- Wi-Fi connectivity
- Built-in web server hosted on the ESP32
- Web dashboard accessible from devices on the local network
- Live sensor data updates using WebSocket
- 7-day weather forecast from an external weather API
- Solar panel statistics from FoxESS
- Local bus departure information from ZKM Gdynia

## Optional Features

- Humidity sensor
- Atmospheric pressure sensor
- Daily temperature chart
- Website dark mode