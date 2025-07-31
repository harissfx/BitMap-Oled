
---

# 🚀 OLED Bitmap Animator

<div align="center">
  <img src="https://img.shields.io/badge/Arduino-Compatible-brightgreen">
  <img src="https://img.shields.io/badge/ESP8266-OK-blue">
  <img src="https://img.shields.io/badge/ESP32-Tested-yellow">
  <img src="https://img.shields.io/badge/License-MIT-red">
</div>

<br>

<p align="center">
  <b>Bikin OLED kamu tampil beda dengan animasi bitmap 🎞️</b><br>
  <i>Proyek ringan untuk menampilkan animasi di OLED SSD1306 menggunakan Arduino atau ESP</i>
</p>

---


* [Fitur](#fitur)
* [Hardware](#hardware)
* [Instalasi](#instalasi)
* [Cara Pakai](#cara-pakai)
* [Kustom Animasi](#kustom-animasi)
* [Troubleshooting](#troubleshooting)
* [Contoh Proyek](#contoh-proyek)
* [Kontribusi](#kontribusi)


---

## ✨ Fitur

* Animasi bitmap berjalan halus (mirip GIF)
* Mendukung berbagai ukuran OLED (128x64, 128x32)
* Hitung frame otomatis, gak perlu ribet
* Penyimpanan efisien dengan `PROGMEM`
* Kompatibel dengan Arduino, ESP8266, dan ESP32

---

## 🔌 Hardware

Perangkat yang diperlukan:

* OLED SSD1306 (I2C)
* Arduino UNO / Nano / ESP8266 / ESP32
* Kabel jumper secukupnya

**Contoh koneksi:**

| OLED Pin | Arduino / ESP Pin |
| -------- | ----------------- |
| GND      | GND               |
| VCC      | 3.3V / 5V         |
| SCL      | A5 / GPIO5        |
| SDA      | A4 / GPIO4        |

---

## ⚙️ Instalasi

1. Buka Arduino IDE
2. Install library berikut melalui **Library Manager**:

   * `Adafruit GFX Library`
   * `Adafruit SSD1306`
3. Pilih board: **Arduino UNO**, **ESP8266**, atau **ESP32**
4. Upload salah satu contoh kode

---

## ▶️ Cara Pakai

1. Clone project ini:

   ```bash
   git clone https://github.com/harissfx/BitMap-Oled.git
   ```
2. Buka file `.ino` di Arduino IDE
3. Upload ke board kamu
4. Lihat hasilnya di OLED 🎉

---

## 🎨 Kustom Animasi

Kamu bisa ganti animasi dengan bitmap sendiri:

* Konversi gambar ke format array dengan tools seperti [image2cpp](https://javl.github.io/image2cpp/)
* Tempel hasilnya di bagian `const unsigned char` di sketch
* Jangan lupa atur ukuran dan jumlah frame

---

## 🧩 Troubleshooting

**OLED tidak menyala?**

* Cek kabel SDA/SCL, pastikan tidak tertukar
* Coba I2C scanner untuk cek alamat I2C

**Gambar tidak pas?**

* Periksa ukuran bitmap
* Sesuaikan resolusi di kode

---

## 📦 Contoh Proyek

* Animasi loading
* Avatar pixel art
* Logo startup

---

## 🤝 Kontribusi

Pull request sangat diterima!
Bisa kirim:

* Perbaikan bug
* Animasi tambahan
* Fitur baru

---

Kalau mau, saya juga bisa bantu buatkan **preview GIF demo OLED-nya** untuk ditaruh di README.
Butuh tambahan bagian **Lisensi**, **Screenshots**, atau **Changelog** juga bisa.
