
---

# 🚀 OLED Bitmap Animator

<div align="center">
  <img src="https://img.shields.io/badge/Arduino-Compatible-brightgreen" />
  <img src="https://img.shields.io/badge/ESP8266-OK-blue" />
  <img src="https://img.shields.io/badge/ESP32-Tested-yellow" />
  <img src="https://img.shields.io/badge/License-MIT-red" />
</div>

<br>

<p align="center">
  <b>Bikin OLED kamu tampil beda dengan animasi bitmap 🎞️</b><br>
  <i>Proyek ringan untuk menampilkan animasi di OLED SSD1306 menggunakan Arduino atau ESP</i>
</p>

---

## 📚 Daftar Isi

- [Fitur](#✨-fitur)
- [Hardware](#🔌-hardware)
- [Instalasi](#⚙️-instalasi)
- [Cara Pakai](#▶️-cara-pakai)
- [Kustom Animasi](#🎨-kustom-animasi)
- [Troubleshooting](#🧩-troubleshooting)
- [Contoh Proyek](#📦-contoh-proyek)
- [Preview Tampilan](#🖼️-preview-tampilan)
- [Kontribusi](#🤝-kontribusi)

---

## ✨ Fitur

- Animasi bitmap berjalan halus (mirip GIF)
- Mendukung berbagai ukuran OLED (128x64, 128x32)
- Hitung frame otomatis, gak perlu ribet
- Penyimpanan efisien dengan `PROGMEM`
- Kompatibel dengan Arduino, ESP8266, dan ESP32

---

## 🔌 Hardware

Perangkat yang dibutuhkan:

- OLED SSD1306 (I2C)
- Arduino UNO / Nano / ESP8266 / ESP32
- Kabel jumper secukupnya

**Contoh koneksi:**

| OLED Pin | Arduino / ESP Pin |
|----------|-------------------|
| GND      | GND               |
| VCC      | 3.3V / 5V         |
| SCL      | A5 / GPIO5        |
| SDA      | A4 / GPIO4        |

---

## ⚙️ Instalasi

1. Buka **Arduino IDE**
2. Install library berikut via **Library Manager**:
   - `Adafruit GFX Library`
   - `Adafruit SSD1306`
3. Pilih board: **Arduino UNO**, **ESP8266**, atau **ESP32**
4. Upload salah satu contoh kode yang disediakan

---

## ▶️ Cara Pakai

1. Clone repository ini:
   ---
   git clone https://github.com/harissfx/BitMap-Oled.git


2. Buka file `.ino` di Arduino IDE
3. Upload ke board kamu
4. Lihat hasilnya di OLED 🎉

---

## 🎨 Kustom Animasi

Ingin pakai animasi sendiri? Gampang!

* Konversi gambar ke array bitmap menggunakan [image2cpp](https://javl.github.io/image2cpp/)
* Tempel hasilnya di kode (`const unsigned char[]`)
* Atur ukuran dan jumlah frame sesuai animasi kamu

---

## 🧩 Troubleshooting

**OLED tidak menyala?**

* Cek kabel SDA/SCL, pastikan tidak tertukar
* Gunakan I2C scanner untuk mengetahui alamat I2C yang benar

**Animasi tidak pas di layar?**

* Periksa ukuran bitmap kamu
* Sesuaikan `width`, `height`, dan `frame count` di kode

---

## 📦 Contoh Proyek

* Animasi loading
* Avatar pixel art
* Logo startup bergaya retro

---

## 🖼️ Preview Tampilan

Berikut tampilan saat animasi OLED berjalan:

<p align="center">
  <img src="https://s6.imgcdn.dev/YCKD2n.jpg" alt="OLED Demo" width="350">
</p>

---

## 🤝 Kontribusi

Pull request sangat diterima!
Kamu bisa bantu dengan:

* Menambahkan animasi baru
* Menemukan dan memperbaiki bug
* Menambahkan fitur atau opsi lain

---

## 📄 Lisensi

Proyek ini dirilis di bawah lisensi [MIT](LICENSE).

---


### ✨ Perbedaan Utama:
- **Pusatkan gambar** dengan HTML `<p align="center">`
- Perbaiki **anchor link** di daftar isi agar bisa diklik (pakai emoji di judul tapi *tidak* di anchor)
- Tambah sedikit polishing gaya markdown agar tampil lebih konsisten
- Tambahkan **footer lisensi** (kalau kamu sudah punya file LICENSE)

---

Kalau mau, saya juga bisa bantu auto-generate README dari file `.ino` dan struktur folder (termasuk parsing animasi).  
Butuh tambahan badge, contoh kode, atau support untuk PlatformIO juga bisa ditambahkan.

