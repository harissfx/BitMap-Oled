# 🚀 OLED Bitmap Animator

<div align="center">
  <img src="https://img.shields.io/badge/Arduino-Compatible-brightgreen">
  <img src="https://img.shields.io/badge/ESP8266-OK-blue">
  <img src="https://img.shields.io/badge/ESP32-Works-yellow">
  <img src="https://img.shields.io/badge/License-MIT-red">
</div>

<br>

<p align="center">
  <b>Animasi keren di OLED kecil? Gas! 💥</b><br>
  <i>Proyek buat nampilin animasi bitmap di OLED SSD1306 pake Arduino/ESP</i>
</p>

---

## 📋 Daftar Isi
- [Fitur Keren](#-fitur-keren)
- [Hardware Needed](#-hardware-yang-dibutuhkan)
- [Installation](#%EF%B8%8F-installasi)
- [Cara Pakai](#-cara-pakai)
- [Custom Animasi](#-custom-animasi)
- [Troubleshooting](#%EF%B8%8F-troubleshooting)
- [Contoh Projek](#-contoh-projek)
- [Contributing](#-contributing)

---

## 🌟 Fitur Keren
✔️ Animasi smooth ala GIF  
✔️ Support multi ukuran OLED (128x64, 128x32, dll)  
✔️ Auto-count frame - gak perlu ngitung manual  
✔️ Hemat RAM pake PROGMEM  
✔️ Compatible Arduino/ESP8266/ESP32  

---

## 🛠️ Hardware yang Dibutuhkan
- OLED SSD1306 (I2C)
- Arduino/ESP8266/ESP32
- Kabel jumper

**Pin Connections:**
| OLED | Arduino/ESP |
|------|-------------|
| GND  | GND         |
| VCC  | 3.3V/5V     |
| SCL  | A5/GPIO5    |
| SDA  | A4/GPIO4    |

---

## ⚙️ Installasi
1. Install library wajib:
   ```arduino
   Adafruit GFX Library
   Adafruit SSD1306
