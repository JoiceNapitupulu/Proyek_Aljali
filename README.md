# Analisis Klastering Performa Siswa (Students Performance Clustering)

Proyek ini bertujuan untuk menganalisis dan mengelompokkan (melakukan klastering) siswa berdasarkan performa akademik mereka menggunakan algoritma **K-Means Clustering**. Dengan memanfaatkan nilai matematika (*math score*), membaca (*reading score*), dan menulis (*writing score*), performa siswa direpresentasikan dalam ruang vektor 3 dimensi ($R^3$) untuk mendapatkan pemahaman yang lebih mendalam mengenai pola belajar dan kelompok akademis siswa.

---

## 🚀 Fitur Utama

- **Representasi Ruang Vektor $R^3$**: Ekstraksi tiga fitur numerik utama (skor matematika, membaca, dan menulis) sebagai koordinat dalam ruang 3 dimensi.
- **Normalisasi Data**: Menggunakan standardisasi (`StandardScaler`) untuk menyamakan skala data sebelum proses klastering agar algoritma berjalan optimal.
- **Klastering dengan K-Means**: Mengelompokkan data siswa menjadi 3 klaster berbeda menggunakan metrik jarak Euclidean.
- **Interpretasi Centroid**: Proses denormalisasi centroid kembali ke skala nilai asli (0-100) untuk mempermudah interpretasi karakteristik akademik tiap kelompok siswa.
- **Visualisasi 3D Interaktif**: Visualisasi sebaran klaster dan titik pusat klaster (centroid) menggunakan grafik scatter 3 dimensi dari Matplotlib.

---

## 🛠️ Teknologi yang Digunakan

Proyek ini dibangun menggunakan bahasa pemrograman **Python** dan beberapa library sains data pendukung:

- **Python 3.10+**
- **Jupyter Notebook** (Format `.ipynb`)
- **Pandas** (Analisis dan manipulasi data)
- **NumPy** (Komputasi numerik)
- **Scikit-Learn** (Preprocessing & Algoritma Machine Learning K-Means)
- **Matplotlib** (Visualisasi data dan plotting 3D)

---

## 📋 Prasyarat Instalasi

Sebelum menjalankan project ini, pastikan Anda telah menginstal Python di sistem Anda. Pasang library yang dibutuhkan dengan menjalankan perintah berikut di terminal/command prompt:

```bash
pip install pandas numpy scikit-learn matplotlib notebook
```

---

## 📁 Struktur Project

Struktur berkas dalam repository ini sangat sederhana:

```text
Proyek_Aljali/
│
├── StudentsPerformance.csv          # Dataset performa akademik siswa
├── Proyek_Aljali_Klastering.ipynb  # Notebook analisis dan proses klastering
└── README.md                       # Dokumentasi proyek (berkas ini)
```

---

## 💻 Contoh Penggunaan

1. **Kloning Repository**
   ```bash
   git clone https://github.com/username/Proyek_Aljali.git
   cd Proyek_Aljali
   ```

2. **Jalankan Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
   Buka file `Proyek_Aljali_Klastering.ipynb` melalui browser.

3. **Alur Kerja Notebook**
   - **Load Data**: Membaca dataset `StudentsPerformance.csv`.
   - **Preprocessing**: Mengekstrak kolom nilai matematika, membaca, dan menulis, lalu menormalisasinya.
   - **Clustering**: Menjalankan K-Means dengan parameter `n_clusters=3`.
   - **Profil Klaster**: Menampilkan pusat klaster (centroid) dalam skala nilai asli, misalnya:
     - **Klaster 0**: Siswa dengan performa akademik rata-rata/menengah (Centroid: Math ~65, Reading ~68, Writing ~68).
     - **Klaster 1**: Siswa yang memerlukan bimbingan lebih/performa akademik rendah (Centroid: Math ~48, Reading ~51, Writing ~48).
     - **Klaster 2**: Siswa berprestasi tinggi/performa akademik tinggi (Centroid: Math ~82, Reading ~85, Writing ~84).
   - **Visualisasi**: Menampilkan grafik scatter 3D untuk melihat sebaran klaster siswa beserta centroid-nya (ditandai dengan huruf `X` merah).

---

## 🤝 Kontribusi

Kontribusi selalu terbuka untuk pengembangan proyek ini. Silakan ikuti langkah-langkah di bawah ini:

1. Lakukan **Fork** pada repository ini.
2. Buat branch fitur baru Anda (`git checkout -b fitur-baru-keren`).
3. Lakukan commit pada perubahan Anda (`git commit -m 'Menambahkan fitur baru yang keren'`).
4. Push ke branch tersebut (`git push origin fitur-baru-keren`).
5. Buat **Pull Request** di GitHub.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **Lisensi MIT** - lihat berkas [LICENSE](file:///d:/KULIAH/SEMESTER%204/ALJALI/Proyek_Aljali/LICENSE) untuk detail selengkapnya.
