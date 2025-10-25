# Panic Buying Detection Model Layer

Repositori ini berisi *notebooks*, model, dan dataset untuk skripsi berjudul **"Identifikasi dan Analisis Perilaku Panic Buying pada Data E-Commerce Menggunakan IndoBERT dan Isolation Forest"**.

Sistem ini dirancang untuk mengidentifikasi dan menganalisis perilaku *panic buying* pada data *e-commerce* Indonesia selama pandemi COVID-19 (2020-2022). Sistem ini memanfaatkan pendekatan dua-tahap:
1.  Model **IndoBERT** yang di-*fine-tune* untuk klasifikasi teks *multi-label* guna mengidentifikasi jenis obat.
2.  Algoritma **Isolation Forest** untuk mendeteksi anomali pada data deret waktu **jumlah ulasan produk mingguan** (yang digunakan sebagai proksi untuk aktivitas pembelian).

---

## 🔧 Tech Stack

* **Python** v3.13.7
* **Torch** v2.6.0
* **Transformers** v.4.52.4 (IndoBERT)
* **Scikit-Learn** v1.7.1 (Isolation Forest, Metrics)
* **Pandas** v2.3.2
* **Numpy** v2.3.2
* **Scipy** v1.16.2 (Pearson Correlation)
* **Matplotlib** v3.10.5
* **Seaborn** v0.13.2
* **Selenium-wire** v5.1.0 (Data Collection)
* **Beautifulsoup4** 4.13.4 (Data Collection)
* **Kaggle Notebooks** (Environment)

---

## 📦 Features

* **Arsitektur Dua-Tahap:** Menggabungkan *fine-tuned* **IndoBERT** untuk klasifikasi teks dan **Isolation Forest** untuk deteksi anomali deret waktu.
* **Time-Series Feature Engineering:** Ekstraksi fitur statistik dan dinamis dari data ulasan mingguan.
* **Validasi Eksternal:** Model divalidasi secara kuantitatif menggunakan **Pearson Correlation** terhadap data *Google Trends* dan secara kualitatif melalui **Analisis Korelasi Naratif** terhadap linimasa berita.
* **Pipeline Pra-pemrosesan Teks:** Termasuk *data integration* (Nama Produk + Deskripsi), *data cleaning* (penghapusan *noise*, duplikat, *missing value*), dan *tokenization* IndoBERT.
* **Metrik Evaluasi (IndoBERT):** F1-score micro, Precision micro, Recall micro, dan Hamming Loss.

---

## 🙏 Acknowledgments

Karya ini merupakan bagian dari Skripsi untuk memenuhi salah satu syarat mencapai gelar sarjana pada Program Studi Teknik Informatika, Fakultas Teknik, Universitas Hasanuddin.

* **Judul:** *Identifikasi dan Analisis Perilaku Panic Buying pada Data E-Commerce Menggunakan IndoBERT dan Isolation Forest*
* **Penulis:** Aidah Dzulfadilah Suwardi (D121211037)
* **Pembimbing:** Ir. Tyanita Puti Marindah W, S.T., M.Inf.
* **Grup Riset:** Distributed Intelligence Research Group