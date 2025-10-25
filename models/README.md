# Model Klasifikasi IndoBERT (Fine-Tuned)

Folder ini berisi file-file yang terkait dengan model IndoBERT yang telah di-*fine-tune* untuk tugas klasifikasi *multi-label* 9 jenis obat, seperti yang dijelaskan dalam penelitian.

## 📦 File Model

Model ini terdiri dari beberapa file konfigurasi dan file bobot (weights) utama:

* **`indobert_medicine_classifier_fixed_model.pth`**: File bobot (weights) model PyTorch yang telah di-*fine-tune*. Ini adalah file utama.
* **`config.json`**: File konfigurasi model.
* **`tokenizer_config.json`**: File konfigurasi tokenizer.
* **`vocab.txt`**: Kosakata (vocabulary) yang digunakan oleh tokenizer.
* File-file pendukung lainnya.

## ‼️ PENTING: Cara Mendapatkan Model

File bobot model (`.pth`) **terlalu besar** untuk disimpan langsung di repositori GitHub ini.

Model ini telah dilatih dan disimpan di platform **Kaggle**. Untuk menjalankan *notebook* klasifikasi (`data_test_classification.ipynb`), Anda harus mengunduh model ini terlebih dahulu.

### 1. Unduh Model dari Kaggle

Anda dapat mengunduh semua file model yang telah dilatih dari tautan publik Kaggle berikut:

**Tautan:** `https://www.kaggle.com/api/v1/datasets/download/aidahdzulfadilah/indobert-medicine-classifier-fixed-model`

*(Pastikan Anda mengikuti instruksi untuk membuat "Kaggle Dataset" baru dari output notebook Anda untuk mendapatkan tautan download publik ini).*

### 2. Tempatkan File Model

Setelah diunduh (dan jika di-zip, silakan di-unzip), pastikan semua file model (termasuk `indobert_medicine_classifier_fixed_model.pth`) ditempatkan di dalam folder yang benar agar *notebook* dapat menemukannya.

Struktur folder yang diharapkan oleh kode adalah:
/models/ | |--- /model/ <-- (Folder ini) | |--- indobert_medicine_classifier_fixed/ | |--- indobert_medicine_classifier_fixed_model.pth | |--- (file-file model lainnya...) | |--- isolation_forest_model.joblib |--- README.md