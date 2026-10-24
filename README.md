# Real-Time Predictive Maintenance for Data Center Infrastructure
# Embedded_IoT_Device
Embedded IoT Device with Edge AI - Smart Predictive Maintenance  

Data center cooling failures are costly and, by the time conventional software tools detect them, hardware damage may already be under way. 
This project presents an independent, out-of-band telemetry platform that monitors the physical health of server cooling fans without consuming any resources on the host server.

An ESP32-S3 microcontroller running MicroPython captures fan vibration (MPU6050 accelerometer) and exhaust-aisle temperature (DHT22 sensor) and streams the readings as JSON over Wi-Fi to a Python 3 analytics server. The server applies Fast Fourier Transform (FFT) signal processing and an unsupervised Isolation Forest model to flag anomalies before they cause downtime, and presents results on a Streamlit dashboard.

