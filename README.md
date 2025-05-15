# ESP32-CAM Motion Detection with Telegram Alerts

This project captures images using an ESP32-CAM when motion is detected via a PIR sensor and sends the image to a Telegram chat.

## Features
- Motion detection via PIR sensor (GPIO 13)
- Captures image with ESP32-CAM
- Sends photo to Telegram using bot API

## Requirements
- ESP32-CAM (AI Thinker)
- PIR motion sensor
- Arduino IDE
- Libraries: WiFi, WiFiClientSecure, ArduinoJson, UniversalTelegramBot

## Setup
1. Connect PIR OUT to GPIO 13, VCC to 3.3V/5V, GND to GND.
2. Create a Telegram bot with [BotFather](https://telegram.me/BotFather) and get the bot token.
3. Get your chat ID by messaging your bot and using Telegram’s getUpdates method.
4. Replace `ssid`, `password`, `token`, and `chat_id` in the code.
5. Flash code to ESP32-CAM using Arduino IDE (select "AI Thinker ESP32-CAM" board).
6. Monitor Serial output for status.

When motion is detected, the ESP32-CAM captures and sends a photo to your Telegram chat.
