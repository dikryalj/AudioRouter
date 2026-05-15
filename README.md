# AudioRouter: Multi-Bluetooth Web Audio Splitter

AudioRouter adalah aplikasi berbasis web (Single-Page Application) yang memungkinkan pengguna untuk mengalirkan audio dari satu sumber ke dua atau lebih perangkat output (seperti headset atau speaker Bluetooth) secara bersamaan. Alat ini dilengkapi dengan fitur kalibrasi latency untuk menyinkronkan suara antar perangkat yang berbeda.

## Demo
https://audio-router-app.vercel.app/ [Hanya bisa pada Laptop]

## 🚀 Fitur Utama

- **Multi-Output Routing**: Alirkan audio ke berbagai perangkat Bluetooth sekaligus langsung dari browser.
- **Drag & Drop Support**: Putar file audio lokal (MP3, WAV) hanya dengan menariknya ke dalam browser.
- **URL Streaming**: Putar audio dari link langsung (Direct Link).
- **Latency Calibration**: Slider delay khusus (0-500ms) untuk setiap perangkat guna memastikan audio terdengar sinkron.
- **Real-time Visualizer**: Visualisasi spektrum audio yang sedang diputar.
- **Dark Mode UI**: Antarmuka modern dan minimalis menggunakan Tailwind CSS.

## 🛠️ Teknologi yang Digunakan

- **Web Audio API**: Inti dari pemrosesan dan perutean audio.
- **MediaDevices API**: Untuk mendeteksi dan memilih perangkat output hardware.
- **Tailwind CSS**: Untuk styling antarmuka yang responsif dan modern.
- **Vanilla JavaScript**: Logika aplikasi murni tanpa framework tambahan.

## 📋 Cara Penggunaan

1. **Persiapan Hardware**: Hubungkan laptop/PC Anda ke dua atau lebih perangkat Bluetooth.
2. **Buka Aplikasi**: Jalankan `index.html` di browser (Disarankan Google Chrome atau Microsoft Edge).
3. **Scan Perangkat**: Klik tombol **"Scan Audio Devices"** dan berikan izin akses audio/mikrofon (diperlukan browser untuk membaca nama hardware).
4. **Input Musik**: Tarik file audio ke area "Drop Zone" atau tempelkan link URL audio langsung.
5. **Aktifkan Output**: Pilih perangkat Bluetooth yang muncul di daftar dengan mencentang checkbox.
6. **Kalibrasi**: Jika suara tidak sinkron, geser slider **Delay** pada perangkat yang terasa lebih cepat.

## ⚠️ Catatan Penting

- **Dukungan Browser**: Fitur `setSinkId` saat ini hanya didukung secara stabil di browser berbasis Chromium (Chrome, Edge, Opera). Safari dan Firefox belum mendukung fitur ini sepenuhnya.
- **Kebijakan CORS**: Streaming dari URL pihak ketiga (seperti YouTube/Spotify) secara langsung dibatasi oleh kebijakan keamanan browser. Gunakan link MP3 langsung atau file lokal untuk hasil terbaik.

## 📄 Lisensi

Proyek ini dibuat untuk tujuan edukasi dan penggunaan pribadi. Silakan kembangkan lebih lanjut!
