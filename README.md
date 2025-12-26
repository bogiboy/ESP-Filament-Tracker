## 🧵 ESP Filament Tracker

A lightweight, web-based filament management system designed for ESP32. Effortlessly manage your 3D printing materials, track remaining stock, and print QR code labels directly from your microcontroller.
✨ Features

ESP32 Support: Full compatibility with the ESP32 family (S2, S3, C3, C6, and classic ESP32).

Web Interface: Fully responsive UI with Dark & Light Mode support for both desktop and mobile.

QR Code Generator: Create labels for your spools that link directly to the filament’s edit menu.

Inventory Management: Store up to 250 filaments with details like manufacturer, material, color, temperature settings, and weight.

Usage Calculator: Easily subtract the weight used after a print to keep your inventory accurate.    

WiFi Captive Portal: Effortless WiFi configuration via a dedicated setup Access Point.

    Backup & Restore: Download your entire database as a binary file and restore it whenever needed.

    Multilingual: Supports both English and German.

## 🛠 Hardware Requirements

    Microcontroller: ESP32 series (S2, S3, C3, C6, or standard ESP32).

    Storage: Utilizes SPIFFS (Serial Peripheral Interface Flash File System) for internal data persistence.

🚀 Installation
1. Web Flasher

Visit the Web Flasher [link your flasher URL here], select your specific board, and click Flash.
2. First-Time Setup (WiFi)

    After flashing, the ESP will create a WiFi Access Point named Filament-Tracker-Setup.

    Connect to this network using your smartphone or PC.

    The setup page should open automatically (Captive Portal). Select your home WiFi network and enter the password.

    The ESP will restart and join your network. It can now be reached via its assigned IP address.

## 📂 File Structure & Data Storage

The tracker manages two main files within the internal flash memory:

    /wifi.txt: Stores your encrypted WiFi credentials.

    /data.bin: A binary file containing the entire filament inventory (struct Filament).

🖥 Screenshots / UI

    Dashboard: Overview of all spools with visual progress bars indicating remaining filament.

    Edit Mode: Adjust temperatures, weights, and manufacturer details.

    QR Label: A print-ready view designed for physical labeling of your filament shelves or spools.

📝 License

This project is released under the MIT License. You are free to use, modify, and distribute it for private and commercial purposes.

## 🚀 Install
If you just want to get started without installing any software, use our Web Flasher:

[![Flash with ESPWebTool](https://img.shields.io/badge/Flash-with%20ESPWebTool-52a552?style=for-the-badge&logo=espressif)](https://www.angelweile.de)

*Supports Chrome and Edge browsers via USB.*

🛠 Hardware Requirements

 Microcontroller: ESP32 series (S2, S3, C3, C6, or standard ESP32).

Storage: Utilizes SPIFFS for internal data persistence.
