# 🏍️ MotoGP Race Results 2022 - 2025 Data Warehouse & Business Intelligence Project

Proyek ini bertujuan untuk membangun Data Warehouse dari dataset MotoGP 2022 serta melakukan analisis data untuk mendapatkan insight terkait performa pembalap, tim, dan hasil balapan.

Dataset yang digunakan berasal dari Kaggle:

https://www.kaggle.com/datasets/sammee/motogp-race-results-2022

---

## 📖 Latar Belakang

MotoGP merupakan salah satu ajang balap motor paling bergengsi di dunia yang memiliki banyak data terkait hasil balapan, pembalap, tim, dan sirkuit.

Namun, data mentah yang tersedia masih belum terstruktur dengan baik untuk kebutuhan analisis. Oleh karena itu, diperlukan proses Data Warehouse untuk mengorganisasi data agar lebih mudah dianalisis.

Dengan adanya Data Warehouse, data dapat digunakan untuk menggali insight seperti:
- Performa pembalap terbaik
- Dominasi tim tertentu
- Hasil balapan di berbagai sirkuit

---

## 🎯 Tujuan

- Membangun Data Warehouse dari dataset MotoGP
- Melakukan proses ETL (Extract, Transform, Load)
- Mengorganisasi data ke dalam bentuk Fact dan Dimension Table
- Melakukan analisis data untuk mendapatkan insight

---

## 👥 Anggota Tim

| 👤 Nama                            | 🎓 NIM     |
|------------------------------------|------------|
| Narendra Augusta Srianandha       | 2409116010 |
| Rahmad Ramadhan                   | 2409116018 |
| Yardan Raditya Rafi' Widyadhana   | 2409116037 |
| Husaini Iyastama H                | 2409116036 |

---

## 📊 Dataset

Dataset yang digunakan adalah MotoGP Race Results 2022 dari Kaggle.

Dataset ini berisi informasi seperti:
- Nama pembalap
- Tim
- Posisi finish
- Waktu balapan
- Sirkuit
- Tanggal balapan

Dataset ini digunakan sebagai sumber utama dalam proses ETL dan pembangunan Data Warehouse.

---

## 🏗️ Data Warehouse Design

Data Warehouse dibangun menggunakan konsep Star Schema yang terdiri dari:

### 📌 Fact Table
- fact_race_results
  - race_id
  - rider_id
  - team_id
  - position
  - points
  - lap_time

### 📌 Dimension Table
- dim_rider
- dim_team
- dim_circuit
- dim_date

Struktur ini memudahkan proses analisis dan query data.

---

## 🔄 ETL Process

### 1. Extract
Data diambil dari dataset Kaggle dalam format CSV.

### 2. Transform
- Membersihkan data (missing value, duplikasi)
- Mengubah format data
- Membuat relasi antar tabel
- Membagi data menjadi fact dan dimension

### 3. Load
Data yang sudah diproses dimasukkan ke dalam struktur Data Warehouse.

---

## 📈 Data Analysis

Beberapa analisis yang dilakukan:

- Pembalap dengan kemenangan terbanyak
- Distribusi posisi finish
- Performa tim berdasarkan hasil balapan
- Analisis sirkuit dengan hasil tercepat

Hasil analisis divisualisasikan menggunakan grafik untuk mempermudah interpretasi data.

---

## 🛠️ Tools & Teknologi

- Python (Pandas, NumPy)
- Jupyter Notebook
- Data Warehouse Modeling
- GitHub

---

## 🚀 Kesimpulan

Dengan membangun Data Warehouse, data MotoGP dapat dianalisis secara lebih efektif dan terstruktur. Insight yang diperoleh dapat membantu dalam memahami performa pembalap dan tim secara lebih mendalam.
