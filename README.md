# ESP32-WROOM-WIFI-AUDITOR
WIFI AUDITOR

Absolutely. Below is a complete ESP32-WROOM Wi-Fi Security Auditor using your OLED + push button + buzzer + breadboard.

This version is designed for a cybersecurity exhibition: it passively scans Wi-Fi networks, identifies their security type, shows signal/channel information, and alerts when an open network is detected. It does not crack passwords or perform deauthentication attacks.


1. Components
> ESP32-WROOM development board
> 0.96" SSD1306 I2C OLED, 128×64
> 1 × push button
> 1 × 3.3 V active buzzer
> Breadboard
> Jumper wires
> USB cable


2. Complete wiring
OLED → ESP32
OLED	ESP32-WROOM
VCC	3V3
GND	GND
SDA	GPIO 21
SCL	GPIO 22
Push button → ESP32
Button	ESP32
One side	GPIO 27
Opposite side	GND

Buzzer → ESP32
Buzzer	ESP32
+	GPIO 25
−	GND


Complete connection
                 ESP32-WROOM
              ┌───────────────┐
              │               │
 OLED VCC ────┤ 3V3           │
 OLED GND ────┤ GND           │
 OLED SDA ────┤ GPIO 21       │
 OLED SCL ────┤ GPIO 22       │
              │               │
 BUTTON ──────┤ GPIO 27       │
 BUTTON ──────┤ GND           │
              │               │
 BUZZER + ────┤ GPIO 25       │
 BUZZER - ────┤ GND           │
              │               │
              └───────────────┘
