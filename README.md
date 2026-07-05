<div align="center">

# 📊 Analisis Statistik Nilai Impor Berdasarkan Golongan Barang Ekonomi (2024)

![Language](https://img.shields.io/badge/Language-Python_3-blue?style=for-the-badge&logo=python&logoColor=white)
![Environment](https://img.shields.io/badge/Environment-Jupyter_Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![Libraries](https://img.shields.io/badge/Libraries-Pandas_%7C_Seaborn_%7C_Matplotlib-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

<p align="center">
  <strong>Proyek data analitik untuk mengevaluasi dinamika nilai impor Indonesia pasca-pandemi berfokus pada Barang Konsumsi dan Bahan Baku Industri.</strong>
</p>

[Tentang Proyek](#-tentang-proyek) • [Tujuan Analisis](#-tujuan-analisis) • [Teknologi](#-spesifikasi-teknologi) • [Visualisasi & Temuan](#-visualisasi--hasil-statistik)

</div>

---

## 📖 Tentang Proyek

Repositori ini memuat *Jupyter Notebook* (`Analisis_Nilai_Impor.ipynb`) yang berfokus pada pengolahan dan visualisasi data makro-ekonomi. Melalui proyek ini, dilakukan komparasi statistik secara deskriptif mengenai performa nilai impor Indonesia sepanjang tahun 2024, yang dibagi ke dalam dua sektor utama: **Barang Konsumsi** dan **Bahan Baku Industri**.

Proyek ini mengekstraksi data secara terstruktur, menghitung parameter statistik inti, dan memproyeksikannya ke dalam grafik agar fluktuasi perekonomian bulanan lebih mudah dipahami oleh pembaca.

---

## 🎯 Tujuan Analisis

Sistem *pipeline* analisis ini dirancang untuk mencapai sasaran berikut:
- 📈 **Perhitungan Statistik Deskriptif:** Melakukan ekstraksi otomatis untuk menemukan *Mean*, *Median*, *Standar Deviasi*, serta titik terendah (MIN) dan tertinggi (MAX) dari data nilai impor.
- 📉 **Pemetaan Tren Temporal:** Melacak pergerakan nilai impor dari Januari hingga Desember 2024 untuk mendeteksi anomali atau siklus pasar.
- 📊 **Komparasi Distribusi Ekstrem:** Membandingkan tingkat penyebaran (dispersi) aliran devisa negara antara sektor konsumtif dengan sektor penunjang manufaktur.

---

## 🛠️ Spesifikasi Teknologi

Logika komputasi dan *rendering* grafis dibangun sepenuhnya menggunakan Python dengan pustaka (*libraries*) standar Data Science:

| Teknologi | Fungsi dalam Proyek |
| :--- | :--- |
| **Pandas** | Ingesti data array, pembuatan DataFrame, restrukturisasi (*melt*), dan agregasi statistik deskriptif (`.describe()`). |
| **Matplotlib** | Membuat kanvas plot (*figure*), merancang garis tren bulanan, dan menambahkan anotasi teks khusus untuk titik ekstrem. |
| **Seaborn** | Modifikasi estetika grafik tingkat tinggi, *grid styling*, dan pembuatan *Boxplot* distribusi. |

---

## 📂 Struktur Repositori

```text
StatistikNilaiImpor/
│
├── 📄 Analisis_Nilai_Impor.ipynb   # Skrip utama berisi kode Python, fungsi pengolahan data, dan visualisasi chart
└── README.md                       # Dokumentasi repositori
```

## 📊 Visualisasi & Hasil Statistik

Skrip ini menghasilkan ringkasan data di terminal dan *output* grafis terstruktur. Berikut adalah temuan utamanya:

### 1. Rekapitulasi Statistik Inti
* **Bahan Baku Industri:** Secara konsisten mendominasi volume transaksi dengan rata-rata nilai **6384.48 Juta US$** dan fluktuasi (Standar Deviasi) sebesar **728.68**. Hal ini mengindikasikan kuatnya arus pasokan material untuk menunjang pabrikasi domestik.
* **Barang Konsumsi:** Cenderung stabil di angka rata-rata **1894.22 Juta US$** per bulan dengan variasi yang lebih rapat (Deviasi: **216.50**).

### 2. Grafik Tren Bulanan (*Line Chart*)
* *Line chart* memetakan perbandingan langsung antara kedua sektor. Algoritma Python menempatkan **Anotasi Pintar (MAX & MIN)** secara otomatis pada titik tertinggi dan terendah dari masing-masing kurva.

### 3. Komparasi Distribusi (*Boxplot*)
* Melalui *Boxplot* yang dihasilkan dari Seaborn, pembaca dapat melihat pemusatan data (kuartil) dan rentang absolutnya. *Boxplot* Bahan Baku Industri memperlihatkan *range* yang jauh lebih luas (*stretched*) dibandingkan Barang Konsumsi yang sangat padat (*compact*).

---

## 🎓 Author

**Cesya Aulia Ramadhani** *Applied Science Undergraduate Student in **Management Informatics** — Universitas Negeri Surabaya*
