# 📘 Modul Pembelajaran Hybrid CEEMDAN–BiLSTM
Prediksi Kunjungan Wisatawan untuk Mendukung Pengelolaan Pariwisata dan Ekonomi Kreatif

## 🗓️ Durasi: 8 Minggu
Modul ini dirancang untuk membantu mahasiswa atau peneliti memahami dan mengimplementasikan model hybrid CEEMDAN–BiLSTM, mulai dari teori dasar hingga eksperimen dan tuning hyperparameter.

---

## 🔹 Minggu 1 – Dasar Statistik dan Time Series
**Tujuan:** Memahami struktur data deret waktu kunjungan wisatawan.

### Materi:
- Trend, musiman, residual
- Uji stasioneritas: ADF, KPSS
- Autocorrelation Function (ACF) dan Partial ACF

### Tugas:
- Uji stasioneritas pada dataset wisatawan (misal data BPS)
- Visualisasi tren dan pola musiman

---

## 🔹 Minggu 2 – Pengenalan EMD, EEMD, dan CEEMDAN
**Tujuan:** Memahami konsep dasar dan perkembangan metode dekomposisi sinyal.

### Materi:
- Empirical Mode Decomposition (EMD) dan Intrinsic Mode Functions (IMF)
- Mode Mixing dan solusi EEMD
- Pengantar CEEMDAN dan adaptive noise

### Tugas:
- Implementasi EMD dan EEMD pada sinyal sederhana
- Studi literatur paper CEEMDAN (Torres et al., 2011)

---

## 🔹 Minggu 3 – Implementasi CEEMDAN dengan Python
**Tujuan:** Menerapkan CEEMDAN secara praktis menggunakan `PyEMD`.

### Materi:
- Instalasi `PyEMD` dan fungsi CEEMDAN
- Parameter penting: noise strength, ensemble size

### Tugas:
- Jalankan CEEMDAN pada data wisatawan
- Visualisasikan dan analisis hasil IMF

---

## 🔹 Minggu 4 – Seleksi dan Pra-pemrosesan IMF
**Tujuan:** Menentukan IMF relevan sebagai input model prediksi.

### Materi:
- Korelasi IMF terhadap sinyal asli
- Teknik normalisasi data time series
- Pembagian data train/test

### Tugas:
- Seleksi IMF berdasarkan korelasi atau varian dominan
- Normalisasi dan persiapan input model

---

## 🔹 Minggu 5 – BiLSTM dan Arsitektur Dasarnya
**Tujuan:** Memahami dasar BiLSTM dan penerapannya pada prediksi.

### Materi:
- Arsitektur LSTM vs BiLSTM
- Input sequence untuk LSTM
- Metrik evaluasi: RMSE, MAE

### Tugas:
- Implementasi BiLSTM sederhana dengan 1 IMF
- Evaluasi prediksi awal

---

## 🔹 Minggu 6 – Integrasi CEEMDAN–BiLSTM
**Tujuan:** Membangun model hybrid menggunakan hasil IMF.

### Materi:
- Strategi input: gabungan semua IMF vs per-IMF
- Prediksi teragregasi dari BiLSTM

### Tugas:
- Latih model dengan kombinasi IMF
- Uji pendekatan kombinasi vs individual IMF

---

## 🔹 Minggu 7 – Hyperparameter Tuning
**Tujuan:** Menyempurnakan performa model melalui tuning.

### Materi:
- Teknik tuning: Grid Search, Random Search, Optuna
- Parameter penting: hidden size, learning rate, timesteps, dropout

### Tugas:
- Lakukan hyperparameter tuning pada model BiLSTM
- Bandingkan hasil tuning vs baseline

---

## 🔹 Minggu 8 – Evaluasi Akhir dan Dokumentasi
**Tujuan:** Menyusun laporan dan memvisualisasikan hasil akhir.

### Materi:
- Evaluasi akhir (MAE, RMSE, MAPE)
- Visualisasi hasil prediksi vs aktual
- Interpretasi hasil model

### Tugas:
- Dokumentasi hasil dalam bentuk laporan mini
- Presentasi hasil model prediksi wisatawan

---

## 📦 Tools yang Disarankan
- Python (3.8+)
- Library: `PyEMD`, `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `tensorflow`/`pytorch`, `optuna`

---

## ✨ Catatan Tambahan
Modul ini cocok digunakan sebagai bagian dari riset akademik atau skripsi, terutama yang berkaitan dengan analisis time series, prediksi wisatawan, atau pengelolaan pariwisata berbasis data.

