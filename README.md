# Temperature-and-Humidity-Monitor-Using-Whatsapp-and-ESP32
Project description

IoT project that enables real-time monitoring of temperature and humidity using an ESP32 microcontroller. The system sends alerts via WhatsApp by integrating Twilio's messaging API and utilizes the ThingESP platform for device management. 

🔧 Project Overview
This project focuses on creating a smart environmental monitoring system that can: 
Measure temperature and humidity using a DHT11 sensor. 
Send real-time alerts to WhatsApp when readings exceed predefined thresholds. 
Utilize Twilio's API for messaging services. 
Manage and monitor the ESP32 device through the ThingESP platform. 
🛠️ Required Components
Wi-Fi Connection 
Twilio Account (for WhatsApp API integration) 
ThingESP Account (for device management) 
⚙️ Setup and Configuration
Hardware Connections: 

Connect the DHT11 sensor to the ESP32: 
VCC to 3.3V 
GND to GND 
DATA to a digital GPIO pin (D7) 
Software Setup: 

Install the Arduino IDE. 
Add the ESP32 board to the Arduino IDE via the Board Manager. 
Install necessary libraries: 

DHT sensor library 
ThingESP library 
WiFi library 
HTTPClient library 
Twilio Configuration:

Sign up for a Twilio account. 
Obtain the Account SID, Auth Token, and a Twilio phone number. 
Set up a WhatsApp sandbox environment in Twilio. 
Configure the webhook URL to point to your server or ThingESP endpoint. 
ThingESP Setup: 

Create an account on ThingESP. 
Register your ESP32 device. 
Obtain the API key and device ID. 
Use these credentials in your Arduino code to authenticate the device. 
Arduino Code: 

Upload the Arduino sketch that is given below: 
Reads data from the DHT11 sensor. 
Connects to Wi-Fi. 
Sends data to ThingESP. 
Triggers WhatsApp messages via Twilio when thresholds are crossed. 
 

📊 Functionality
The ESP32 continuously reads temperature and humidity data from the DHT11 sensor. 
Data is sent to ThingESP for monitoring and logging. 
If readings exceed set thresholds (e.g., temperature > 30°C), the ESP32 sends an HTTP request to Twilio's API. 
Twilio then sends a WhatsApp message to the configured number, alerting the user of the condition. 
 

 

This project is an excellent example of integrating hardware and cloud services to create a responsive and accessible monitoring system. By leveraging WhatsApp for notifications, it ensures that alerts are delivered promptly and are easily accessible to users. 

 
