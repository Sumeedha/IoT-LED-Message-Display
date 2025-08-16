# IoT-LED-Message-Display

This project is a Smart Notice Board built using NodeMCU ESP8266, P10 LED Matrix Display, and the Blynk IoT platform.
It allows messages to be updated wirelessly via mobile app or web dashboard and displayed on the LED board.

𝗣𝗿𝗼𝗷𝗲𝗰𝘁 𝗚𝘂𝗶𝗱𝗮𝗻𝗰𝗲 𝗩𝗶𝗱𝗲𝗼:https://www.youtube.com/watch?v=hns8wvBJLts

🚀 𝗙𝗲𝗮𝘁𝘂𝗿𝗲𝘀

Wireless message update via Blynk IoT app / web dashboard
Supports scrolling & static text modes
Adjustable text scrolling speed
Cost-effective & scalable solution
Applications: Schools, Colleges, Banks, Public Places

🛠️ 𝗖𝗼𝗺𝗽𝗼𝗻𝗲𝗻𝘁𝘀 𝗥𝗲𝗾𝘂𝗶𝗿𝗲𝗱

NodeMCU ESP8266 / ESP32
P10 LED Matrix Display
Jumper Wires
Power Supply (5V)
Breadboard (optional)

🔌 𝐇𝐚𝐫𝐝𝐰𝐚𝐫𝐞 𝐂𝐨𝐧𝐧𝐞𝐜𝐭𝐢𝐨𝐧𝐬
Refer to the circuit diagram in /images/circuit_diagram.png

📂 𝐑𝐞𝐩𝐨𝐬𝐢𝐭𝐨𝐫𝐲 𝐂𝐨𝐧𝐭𝐞𝐧𝐭𝐬

Arduino Code
Project Report (PDF)
Demo Video
README.md
LICENSE

🌐 𝐁𝐥𝐲𝐧𝐤 𝐈𝐨𝐓 𝐒𝐞𝐭𝐮𝐩

Follow these steps to configure Blynk Cloud for the IoT LED Message Display project:

🔑 𝐒𝐭𝐞𝐩 𝟏: 𝐂𝐫𝐞𝐚𝐭𝐞/𝐋𝐨𝐠𝐢𝐧 𝐭𝐨 𝐁𝐥𝐲𝐧𝐤 𝐀𝐜𝐜𝐨𝐮𝐧𝐭
Open Blynk Cloud.
Login or create a new account.

📝 𝐒𝐭𝐞𝐩 𝟐: 𝐂𝐫𝐞𝐚𝐭𝐞 𝐚 𝐍𝐞𝐰 𝐓𝐞𝐦𝐩𝐥𝐚𝐭𝐞
Template Name: LED Matrix Control using Blynk IoT
Hardware: ESP8266 (or ESP32)
Connection: Wi-Fi
Description: LED Matrix Control

📊 𝐒𝐭𝐞𝐩 𝟑: 𝐂𝐫𝐞𝐚𝐭𝐞 𝐃𝐚𝐭𝐚 𝐒𝐭𝐫𝐞𝐚𝐦𝐬
V0 → Message (String)
V1 → Scrolling Speed (String)

🖥️ 𝐒𝐭𝐞𝐩 𝟒: 𝐂𝐨𝐧𝐟𝐢𝐠𝐮𝐫𝐞 𝐖𝐞𝐛 𝐃𝐚𝐬𝐡𝐛𝐨𝐚𝐫𝐝
Add Terminal widgets
V0 → Title: Type your message here
V1 → Title: Enter scrolling speed

📱 𝐒𝐭𝐞𝐩 𝟓: 𝐀𝐝𝐝 𝐃𝐞𝐯𝐢𝐜𝐞
Add new device → From Template → Choose template
Copy Auth Token, Template ID, Device Name

💻 𝐒𝐭𝐞𝐩 𝟔: 𝐀𝐫𝐝𝐮𝐢𝐧𝐨 𝐂𝐨𝐝𝐞

Update the credentials in code:

#define BLYNK_TEMPLATE_ID   "Your Template ID"
#define BLYNK_DEVICE_NAME   "Your Device Name"
#define BLYNK_AUTH_TOKEN    "Your Auth Token"

char ssid[] = "Your WiFi SSID";
char pass[] = "Your WiFi Password";


Upload to NodeMCU ESP8266 → Test with Blynk App/Web.

⚙️ 𝐈𝐧𝐬𝐭𝐚𝐥𝐥𝐚𝐭𝐢𝐨𝐧 & 𝐔𝐬𝐚𝐠𝐞

1)Open the code in Arduino IDE

2)Install libraries: Blynk, ESP8266WiFi

3)Select NodeMCU 1.0 (ESP8266) board

4)Upload code → Open Blynk app → Control LED matrix

🙏 𝐀𝐜𝐤𝐧𝐨𝐰𝐥𝐞𝐝𝐠𝐞𝐦𝐞𝐧𝐭

This project was implemented by following the guidance from this YouTube tutorial.
The source code was adapted from the tutorial and uploaded here for educational and learning purposes.

📜 𝐋𝐢𝐜𝐞𝐧𝐬𝐞

This project is licensed under the MIT License.
You are free to use, modify, and share it with attribution.
