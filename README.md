# 🚁 DJI Tello Controller (Ionic + Cordova)

![GitHub repo size](https://img.shields.io/github/repo-size/zhafraz/DJI_Tello_Controller_IonicCordova?color=4CAF50)
![GitHub last commit](https://img.shields.io/github/last-commit/zhafraz/DJI_Tello_Controller_IonicCordova?color=2196F3)
![GitHub top language](https://img.shields.io/github/languages/top/zhafraz/DJI_Tello_Controller_IonicCordova?color=FF9800)
![GitHub stars](https://img.shields.io/github/stars/zhafraz/DJI_Tello_Controller_IonicCordova?style=social)

Aplikasi **DJI Tello Controller** dibuat menggunakan **Ionic Framework + Apache Cordova** untuk mengontrol drone **DJI Tello** secara langsung melalui jaringan Wi-Fi.  
Proyek ini mendemonstrasikan integrasi antara **mobile hybrid app** dan **UDP communication** untuk mengirim perintah ke drone.

---

## ⚙️ Fitur Utama

✅ Menghubungkan perangkat ke jaringan Wi-Fi drone DJI Tello  
✅ Mengirim perintah terbang (takeoff, land, flip, dll)  
✅ Menampilkan status koneksi drone secara real-time  
✅ Menampilkan *live telemetry* (baterai, tinggi, status terbang)  
✅ UI berbasis **Ionic + Angular** dengan tampilan responsif  
✅ Dukungan **Cordova plugin** untuk akses jaringan UDP

---

## 🧠 Teknologi yang Digunakan

| Teknologi | Keterangan |
|:-----------|:------------|
| **Ionic Framework** | Front-end framework untuk aplikasi mobile hybrid |
| **Apache Cordova** | Untuk kompilasi aplikasi ke Android/iOS |
| **TypeScript** | Bahasa utama proyek |
| **Node.js + NPM** | Manajemen paket dan dependensi |
| **UDP Socket** | Protokol komunikasi dengan DJI Tello |

---

## 🚀 Cara Menjalankan Proyek

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/zhafraz/DJI_Tello_Controller_IonicCordova.git
   cd DJI_Tello_Controller_IonicCordova

2. **Instal dependensi:**
   ```bash
   npm install

3. **Jalankan dalam mode pengembangan (browser):**

   ```bash
   ionic serve

4. **Untuk menjalankan di perangkat Android:**

   ```bash
   ionic cordova platform add android
   ionic cordova run android

5. **Hubungkan perangkat ke Wi-Fi DJI Tello**, lalu jalankan aplikasi.
   💡 *Pastikan alamat IP dan port UDP sudah disesuaikan di file konfigurasi.*

---

## 📂 Struktur Folder

| Folder                | Deskripsi                                                   |
| :-------------------- | :---------------------------------------------------------- |
| **src/**              | Berisi kode utama aplikasi (komponen, halaman, dan service) |
| **src/app/services/** | Modul komunikasi UDP dengan DJI Tello                       |
| **src/pages/**        | Tampilan utama aplikasi (Controller, Status, Settings)      |
| **www/**              | File hasil build siap untuk Cordova                         |

---


## 🧩 Catatan Teknis

* Default IP DJI Tello: `192.168.10.1`
* Command port: `8889`
* Video port (optional): `11111`
* Telemetry port: `8890`

Jika ingin menambahkan fitur *video streaming*, gunakan decoding H.264 melalui library tambahan seperti `ffmpeg.js` atau integrasi ke server lokal untuk decoding stream UDP.

---
