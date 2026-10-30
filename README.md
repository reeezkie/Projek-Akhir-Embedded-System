# 🔥 FIRESENTRY: Mitigasi Kebakaran Dini Berbasis IoT & Embedded System
> Sistem Deteksi Dini & Mitigasi Kebakaran Terintegrasi Berbasis Mikrokontroler ESP32 & Sensor Fusion

[![Status Project](https://img.shields.io/badge/Status-Completed-success.svg)]()
[![Embedded C++](https://img.shields.io/badge/Language-C%2F++%20%2F%20Arduino-blue.svg)]()
[![Institution](https://img.shields.io/badge/Universitas-Brawijaya-red.svg)]()

Repositori ini berisi dokumentasi lengkap, skematik hardware, kode sumber, dan laporan akhir untuk proyek mata kuliah **Embedded System**. Proyek ini berfokus pada perancangan sistem tertanam (*embedded system*) mandiri yang mengintegrasikan multisensor, metode *sensor fusion*, peringatan audio-visual lokal, serta komunikasi IoT via MQTT dan Telegram Bot untuk mitigasi kebakaran dini.

---

## 🏛️ Informasi Akademik
* **Mata Kuliah:** Embedded System (Sistem Tertanam)
* **Institusi:** Fakultas Ilmu Komputer, Universitas Brawijaya (FILKOM UB)
* **Tahun Akademik:** 2026

---

## 👥 Tim Penyusun (Sesuai Dokumen Laporan)
Proyek ini dikerjakan oleh kelompok yang beranggotakan:
1. **Rezky Auliasarie** (245150300111014)
2. **Agatha Triotama** (245150300111020)
3. **Zeyra Rahma Alivia** (245150301111016)
4. **Muhammad Naufal M. R** (245150307111006)
5. **Delvin Nhean Olamina** (245150307111032)

---

## 💡 Latar Belakang & Tujuan
Bahaya kebakaran akibat korsleting listrik, kebocoran gas, maupun keterlambatan deteksi dini sering kali memicu kerugian material dan korban jiwa. **FIRESENTRY** dikembangkan untuk merancang sistem pemantauan lingkungan berbasis *embedded system* yang handal. 

Sistem ini menerapkan metode ***sensor fusion*** dari multisensor guna meminimalkan *false alarm*, dilengkapi mekanisme respons mitigasi aktif berupa alarm audio-visual lokal (Buzzer, LED RGB, OLED Display), serta transmisi data darurat berlatensi rendah secara *real-time* ke platform IoT (MQTT Broker & Telegram Bot API).

---

## 🛠️ Komponen & Teknologi Utama
* **Mikrokontroler:** ESP32 DevKit (Pusat pemrosesan & modul WiFi terintegrasi)
* **Sensor:** 
  * Flame IR Sensor (Deteksi radiasi inframerah nyala api via *digital interrupt*)
  * MQ-2 Gas & Smoke Sensor (Deteksi gas mudah terbakar & asap via ADC 12-bit)
  * DS18B20 (Sensor suhu digital presisi tinggi berbasis protokol OneWire)
* **Aktuator & Display:** OLED Display 0,96" (I2C), Buzzer (Alarm audio intermiten/kontinu), LED RGB (Indikator status AMAN, ALERT, BAHAYA)
* **Komunikasi & IoT:** MQTT Protocol over TLS (HiveMQ Cloud), Telegram Bot API (Notifikasi *urgent alert* format JSON), Arduino IDE

---

## 📂 Struktur Repositori
```text
├── LAPORAN AKHIR PROJECT EMBEDDED SYSTEM (1).pdf    # Dokumen laporan lengkap (arsitektur, perancangan, skematik, & pengujian)
└── README.md                                        # Dokumentasi proyek
