
IoT Pulse Oximeter with ThingSpeak Integration
This project is an IoT-enabled pulse oximeter that monitors heart rate and SpO2 levels using the MAX30100 sensor and ESP8266. It displays data on an OLED screen and uploads readings to ThingSpeak for real-time remote monitoring. Ideal for health tracking, wearables, and IoT learning.

Features
Real-time heart rate and SpO2 monitoring
OLED display for local data visualization
WiFi-enabled ThingSpeak integration for remote monitoring
Automatic error handling and sensor reset
Wiring Instructions
MAX30100 Sensor:

VIN to 3.3V on ESP8266
GND to GND on ESP8266
SCL to D1 (GPIO5) on ESP8266
SDA to D2 (GPIO4) on ESP8266
OLED Display:

VCC to 3.3V on ESP8266
GND to GND on ESP8266
SCL to D1 (GPIO5) on ESP8266
SDA to D2 (GPIO4) on ESP8266
Note: Both the MAX30100 and OLED display share the same I2C pins (SCL and SDA), allowing them to be connected in parallel.

Software Requirements
Arduino IDE: Use the Arduino IDE to write, compile, and upload code to the ESP8266.
Libraries: Install the following libraries through the Arduino Library Manager or GitHub:
ESP8266WiFi
ThingSpeak
MAX30100_PulseOximeter
Adafruit_GFX
Adafruit_SSD1306
USB and Driver Requirements
USB Port: Connect the ESP8266 to your computer via a micro-USB cable.
Driver: For the ESP8266 to communicate with the Arduino IDE on Windows, you may need to install the CP210x USB to UART Bridge VCP driver.
Download and install the driver from the Silicon Labs website.
Setup
Clone the repository.
Open the Arduino IDE, then open the .ino file.
Update WiFi and ThingSpeak credentials in the code.
Select NodeMCU 1.0 (ESP-12E Module) in the board settings.
Choose the correct COM port (visible after driver installation).
Upload the code to ESP8266 and start monitoring.
