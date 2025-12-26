## 🧵 ESP Filament Tracker

A lightweight, web-based filament management system designed for ESP32. Effortlessly manage your 3D printing materials, track remaining stock, and print QR code labels directly from your microcontroller.
✨ Features

    ESP32 Support: Full compatibility with the ESP32 family ( S3, C3, C6, and classic ESP32).

    Web Interface: Fully responsive UI with Dark & Light Mode support for both desktop and mobile.

    QR Code Generator: Create labels for your spools that link directly to the filament’s edit menu.

    Inventory Management: Store up to 250 filaments with details like manufacturer, material, color, temperature settings, and weight.

    Usage Calculator: Easily subtract the weight used after a print to keep your inventory accurate.

    Smart Progress Bar: The color-coded bar on each filament card automatically shrinks as the remaining weight decreases.

    The bar reflects the percentage of filament left (based on a standard 1kg spool), giving you an instant overview of which spools are running low.

    WiFi Captive Portal: Effortless WiFi configuration via a dedicated setup Access Point.

    Backup & Restore: Download your entire database as a binary file and restore it whenever needed.

    30-Day Backup Reminder: The tracker automatically monitors the time since your last data export.

    Multilingual: Supports both English and German.




##    🏷️ Smart QR-Code Labels & Export

The ESP Filament Tracker doesn't just store data; it bridges the gap between your digital inventory and your physical spools. Each filament entry can generate a custom, print-ready label.
What’s on the Label?

The generated label is optimized for clarity and includes all essential information for a successful print:

    Manufacturer & Material: Large, bold text for quick identification.

    Dynamic QR-Code: A scanable code that links directly to the specific filament's edit page on your ESP32.

    Temperature Profiles: Printed values for both Nozzle (Hotend) and Print Bed ranges.

    Print-Ready Format: A clean, black-and-white design optimized for standard thermal label printers or regular paper.

How it Improves your Workflow

    Instant Access: Instead of searching through a long list, simply scan the QR code on the physical spool with your smartphone camera.

    Direct Editing: The scan takes you directly to the edit page where you can instantly subtract the weight used after a print.

    No More Guesswork: All technical data (temperatures) is physically attached to the spool, so you don't have to look up the manufacturer's specs ever again.

## 🛠 Hardware Requirements

    Microcontroller: ESP32 series (S3, C3, C6, or standard ESP32).

    Storage: Utilizes SPIFFS (Serial Peripheral Interface Flash File System) for internal data persistence.

## 🚀 Installation
1. Web Flasher

Visit the Web Flasher [![Flash with ESPWebTool](https://img.shields.io/badge/Flash-with%20ESPWebTool-52a552?style=for-the-badge&logo=espressif)](https://www.angelweile.de), select your specific board, and click Flash.
2. First-Time Setup (WiFi)

    After flashing, the ESP will create a WiFi Access Point named Filament-Tracker-Setup.

    Connect to this network using your smartphone or PC.

    The setup page should open automatically (Captive Portal). Select your home WiFi network and enter the password.

    The ESP will restart and join your network. It can now be reached via its assigned IP address.

📂 File Structure & Data Storage

The tracker manages two main files within the internal flash memory:

    /wifi.txt: Stores your encrypted WiFi credentials.

    /data.bin: A binary file containing the entire filament inventory (struct Filament).

🖥 Screenshots / UI

    Dashboard: Overview of all spools with visual progress bars indicating remaining filament.

    Edit Mode: Adjust temperatures, weights, and manufacturer details.

    QR Label: A print-ready view designed for physical labeling of your filament shelves or spools.

![Login Screenshot](https://github.com/bogiboy/ESP-Filament-Tracker/blob/main/screenshots/dunkel.png)
![Login Screenshot](https://github.com/bogiboy/ESP-Filament-Tracker/blob/main/screenshots/liste.png)
![Login Screenshot](https://github.com/bogiboy/ESP-Filament-Tracker/blob/main/screenshots/edit.png)
![Login Screenshot](https://github.com/bogiboy/ESP-Filament-Tracker/blob/main/screenshots/hell.png)
![Login Screenshot](https://github.com/bogiboy/ESP-Filament-Tracker/blob/main/screenshots/qrcode.png)

📝 License

This project is released under the MIT License. You are free to use, modify, and distribute it for private and commercial purposes.


