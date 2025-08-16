# IoT-LED-Message-Display

This project is a Smart Notice Board built using NodeMCU ESP8266, P10 LED Matrix Display, and the Blynk IoT platform.
It allows messages to be updated wirelessly via mobile app or web dashboard and displayed on the LED board.

Project Guidance Video:https://www.youtube.com/watch?v=hns8wvBJLts

🚀 Features

Wireless message update via Blynk IoT app / web dashboard
Supports scrolling & static text modes
Adjustable text scrolling speed
Cost-effective & scalable solution
Applications: Schools, Colleges, Banks, Public Places

🛠️ Components Required

NodeMCU ESP8266 / ESP32
P10 LED Matrix Display
Jumper Wires
Power Supply (5V)
Breadboard (optional)

🔌 Hardware Connections
Refer to the circuit diagram in /images/circuit_diagram.png

📂 Repository Contents

Arduino Code
Project Report (PDF)
Demo Video
README.md
LICENSE

🌐 Blynk IoT Setup

Follow these steps to configure Blynk Cloud for the IoT LED Message Display project:

🔑 Step 1: Create/Login to Blynk Account
Open Blynk Cloud.
Login or create a new account.

📝 Step 2: Create a New Template
Template Name: LED Matrix Control using Blynk IoT
Hardware: ESP8266 (or ESP32)
Connection: Wi-Fi
Description: LED Matrix Control

📊 Step 3: Create Data Streams
V0 → Message (String)
V1 → Scrolling Speed (String)

🖥️ Step 4: Configure Web Dashboard
Add Terminal widgets
V0 → Title: Type your message here
V1 → Title: Enter scrolling speed

📱 Step 5: Add Device
Add new device → From Template → Choose template
Copy Auth Token, Template ID, Device Name

💻 Step 6: Arduino Code

Update the credentials in code:

#define BLYNK_TEMPLATE_ID   "Your Template ID"
#define BLYNK_DEVICE_NAME   "Your Device Name"
#define BLYNK_AUTH_TOKEN    "Your Auth Token"

char ssid[] = "Your WiFi SSID";
char pass[] = "Your WiFi Password";


Upload to NodeMCU ESP8266 → Test with Blynk App/Web.

⚙️ Installation & Usage

Open the code in Arduino IDE
Install libraries: Blynk, ESP8266WiFi
Select NodeMCU 1.0 (ESP8266) board
Upload code → Open Blynk app → Control LED matrix

🙏 Acknowledgement

This project was implemented by following the guidance from this YouTube tutorial.
The source code was adapted from the tutorial and uploaded here for educational and learning purposes.

📜 License

This project is licensed under the MIT License.
You are free to use, modify, and share it with attribution.
