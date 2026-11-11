# Project Deep Learning - SDGs 12 Konsumsi dan Produksi yang Bertanggung Jawab

## ♻️ Implementasi Transfer Learning Berbasis CNN untuk Klasifikasi Jenis Sampah di Lingkungan Kampus

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

Proyek ini berkaitan dengan **SDG 12: Responsible Consumption and Production (Konsumsi dan Produksi yang Bertanggung Jawab)**.

SDG 12 menekankan pentingnya pola konsumsi dan produksi yang bertanggung jawab, termasuk pengurangan limbah serta peningkatan pengelolaan sampah.

Melalui penerapan teknologi Deep Learning, proyek ini mendukung proses identifikasi jenis sampah sebagai salah satu upaya untuk meningkatkan kesadaran dan efektivitas pemilahan sampah.

---

## 👥 Anggota Kelompok

| No. | Nama Anggota | NIM |
|---|---|---|
| 1 | Elsya Sagitha Damayanti S | F1G125029 |
| 2 | Rahmah Hidayah Lahompu | F1G125047 |
| 3 | Ridha Septiani K | F1G125075 |

**Program Studi Ilmu Komputer**  
**Fakultas Matematika dan Ilmu Pengetahuan Alam**  
**Universitas Halu Oleo**

---

## 📌 Deskripsi Proyek

Proyek ini merupakan implementasi Deep Learning untuk mengembangkan sistem klasifikasi otomatis jenis sampah berdasarkan citra gambar (*image classification*).

Sistem dirancang untuk mengenali dan mengelompokkan berbagai jenis sampah berdasarkan karakteristik visualnya, seperti bentuk, warna, tekstur, dan pola.

Pengembangan sistem menggunakan pendekatan **Transfer Learning** berbasis **Convolutional Neural Network (CNN)** dengan framework **TensorFlow**. Model *pre-trained* **MobileNetV2** dimanfaatkan dan disesuaikan dengan dataset gambar sampah, kemudian ditingkatkan melalui proses **fine-tuning**. Model akhir diintegrasikan ke dalam aplikasi web sederhana berbasis **Streamlit** sehingga dapat digunakan untuk mengklasifikasikan gambar sampah secara langsung.

Proyek ini berfokus pada pemanfaatan teknologi Artificial Intelligence (AI) untuk membantu proses identifikasi dan pemilahan sampah, khususnya dalam konteks lingkungan perguruan tinggi.

## 🎯 Latar Belakang

Sampah merupakan salah satu permasalahan lingkungan yang masih sering dijumpai, termasuk di lingkungan perguruan tinggi. Berbagai aktivitas akademik dan kegiatan sehari-hari menghasilkan beragam jenis sampah, seperti plastik, kertas, kardus, kaca, logam, dan sampah organik.

Namun, proses pemilahan sampah masih menjadi tantangan karena kurangnya pengetahuan mengenai pengelompokan sampah berdasarkan jenis materialnya. Sampah yang tercampur dapat menyulitkan proses pengelolaan dan daur ulang.

Seiring perkembangan teknologi Artificial Intelligence, khususnya Deep Learning, klasifikasi citra dapat dimanfaatkan untuk membantu mengenali berbagai jenis sampah secara otomatis berdasarkan karakteristik visualnya.

Melalui proyek ini, diterapkan metode Transfer Learning berbasis CNN menggunakan TensorFlow untuk mengembangkan model yang mampu mengklasifikasikan jenis sampah berdasarkan gambar, sebagai bentuk pemanfaatan teknologi AI dalam mendukung pengelolaan sampah serta meningkatkan kesadaran terhadap pentingnya pemilahan sampah di lingkungan kampus.

## 🎯 Tujuan Proyek

1. Mengimplementasikan metode Transfer Learning berbasis CNN untuk klasifikasi jenis sampah.
2. Mengembangkan model Deep Learning menggunakan TensorFlow.
3. Mengidentifikasi berbagai kategori sampah berdasarkan citra gambar.
4. Mengevaluasi performa model berdasarkan hasil pengujian.
5. Menerapkan teknologi Artificial Intelligence sebagai pendukung proses identifikasi dan pemilahan sampah melalui aplikasi web.

## ❓ Rumusan Masalah

1. Bagaimana menerapkan metode Transfer Learning berbasis CNN menggunakan TensorFlow untuk mengklasifikasikan jenis sampah berdasarkan gambar?
2. Bagaimana model Deep Learning dapat mengenali dan membedakan berbagai jenis sampah berdasarkan karakteristik visualnya?
3. Bagaimana performa model Transfer Learning dalam mengklasifikasikan berbagai kategori sampah?
4. Bagaimana hasil klasifikasi otomatis dapat dimanfaatkan untuk membantu proses pemilahan sampah di lingkungan kampus?

---

## 🗑️ Dataset

Dataset yang digunakan dalam proyek ini adalah **RealWaste Dataset** yang diperoleh melalui platform Kaggle.

🔗 **Sumber Dataset:** [RealWaste - Kaggle](https://www.kaggle.com/datasets/joebeachcapital/realwaste)

RealWaste merupakan dataset citra sampah yang berisi gambar berbagai jenis material sampah. Dataset ini digunakan untuk melatih dan menguji kemampuan model dalam mengenali serta mengklasifikasikan jenis sampah berdasarkan karakteristik visualnya.

### 📊 Informasi Dataset

| Keterangan | Detail |
|---|---|
| Nama Dataset | RealWaste |
| Sumber | Kaggle |
| Total Gambar | 4.752 gambar |
| Jumlah Kategori | 9 kelas |
| Format Gambar | RGB |
| Resolusi | 524 × 524 piksel |
| Jenis Tugas | Image Classification |

### 🏷️ Kategori Klasifikasi

| No. | Kategori | Jumlah Gambar |
|---|---|---:|
| 1 | Cardboard | 461 |
| 2 | Food Organics | 411 |
| 3 | Glass | 420 |
| 4 | Metal | 790 |
| 5 | Miscellaneous Trash | 495 |
| 6 | Paper | 500 |
| 7 | Plastic | 921 |
| 8 | Textile Trash | 318 |
| 9 | Vegetation | 436 |
| | **Total** | **4.752** |

### ✂️ Pembagian Dataset

Dataset dibagi menggunakan library `split-folders` dengan `seed=42` agar hasil pembagian dapat direproduksi.

| Bagian | Proporsi | Jumlah Gambar |
|---|---|---:|
| Training Set | 70% | 3.323 |
| Validation Set | 15% | 710 |
| Testing Set | 15% | 719 |

---

## 🧠 Metode dan Teknologi

### 1. Transfer Learning

Transfer Learning merupakan pendekatan pembelajaran mesin yang memanfaatkan pengetahuan dari model yang telah dilatih sebelumnya (*pre-trained model*) untuk menyelesaikan tugas baru. Pendekatan ini digunakan agar model klasifikasi sampah dapat memanfaatkan fitur visual yang telah dipelajari dari dataset sebelumnya.

### 2. Convolutional Neural Network (CNN)

CNN merupakan arsitektur Deep Learning yang banyak digunakan dalam pengolahan citra. CNN mampu mempelajari karakteristik visual gambar melalui proses ekstraksi fitur, seperti bentuk, tekstur, dan pola.

### 3. MobileNetV2

Model yang digunakan adalah **MobileNetV2** dengan bobot *pre-trained* dari **ImageNet**. MobileNetV2 dirancang agar lebih ringan dan efisien dalam pemrosesan citra.

Arsitektur model yang dibangun:

| Lapisan | Fungsi |
|---|---|
| MobileNetV2 (tanpa lapisan klasifikasi bawaan) | Ekstraksi fitur visual |
| GlobalAveragePooling2D | Meringkas *feature map* menjadi satu vektor fitur |
| Dropout (0,2) | Mengurangi risiko *overfitting* |
| Dense (9, softmax) | Menghasilkan probabilitas untuk 9 kategori sampah |

### 4. Fine-Tuning

Setelah pelatihan awal (MobileNetV2 dibekukan), 30 lapisan terakhir MobileNetV2 dibuka (kecuali lapisan *BatchNormalization*) dan dilatih ulang selama 15 epoch dengan *learning rate* 0,00001 agar bobot model lebih sesuai dengan dataset RealWaste.

### 🛠️ Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| Bahasa Pemrograman | Python |
| Framework Deep Learning | TensorFlow / Keras |
| Metode | Transfer Learning dan Fine-Tuning |
| Arsitektur CNN | MobileNetV2 |
| Pengembangan Model | Google Colab |
| Pengunduhan Dataset | KaggleHub |
| Pembagian Dataset | split-folders |
| Pengolahan Data | NumPy, Pillow |
| Visualisasi | Matplotlib |
| Evaluasi Model | Scikit-learn |
| Aplikasi Web | Streamlit |
| Version Control | Git & GitHub |

---

## ⚙️ Tahapan Pengembangan

### 1. Pengumpulan Dataset
Mengunduh dataset RealWaste dari Kaggle menggunakan `kagglehub`.

### 2. Exploratory Data Analysis (EDA)
Mengeksplorasi struktur dataset, jumlah gambar setiap kategori, serta menampilkan contoh gambar dari setiap kelas. Dari tahap ini terlihat bahwa distribusi kelas tidak seimbang (Plastic 921 gambar vs Textile Trash 318 gambar).

### 3. Pembagian Dataset
Membagi dataset menjadi training (70%), validation (15%), dan testing (15%).

### 4. Preprocessing Data
- Memuat gambar dari folder dengan ukuran 224 × 224 piksel dan *batch size* 32.
- Normalisasi nilai piksel menggunakan `preprocess_input` MobileNetV2 ke rentang [-1, 1].
- Pemeriksaan hasil normalisasi.

### 5. Implementasi Transfer Learning
Menggunakan MobileNetV2 *pre-trained* (ImageNet) yang dibekukan, kemudian menambahkan lapisan klasifikasi untuk sembilan kategori sampah.

### 6. Training Model
Melatih lapisan klasifikasi selama 10 epoch menggunakan optimizer Adam dan loss *sparse categorical crossentropy*.

### 7. Evaluasi Awal
Mengukur performa model pada data testing menggunakan accuracy, classification report, dan confusion matrix.

### 8. Fine-Tuning
Membuka 30 lapisan terakhir MobileNetV2 dan melatih ulang model selama 15 epoch dengan *learning rate* 0,00001.

### 9. Evaluasi Setelah Fine-Tuning
Mengevaluasi kembali model pada data testing dan membandingkannya dengan hasil sebelum fine-tuning.

### 10. Penyimpanan Model
Menyimpan model dalam format `.keras` (`waste_classifier.keras`) dan nama kelas dalam `class_names.json`.

### 11. Pengujian Gambar Baru
Menguji model menggunakan gambar sampah baru yang belum pernah digunakan pada proses training, lengkap dengan kategori prediksi dan probabilitas untuk setiap kelas.

### 12. Pembuatan Aplikasi Web
Membangun aplikasi klasifikasi sampah berbasis Streamlit (`app.py`) yang memuat model, menerima gambar unggahan, lalu menampilkan kategori prediksi, *confidence score*, dan probabilitas setiap kategori.

---

## 📊 Hasil Evaluasi Model

Model dievaluasi pada 719 gambar data testing menggunakan accuracy, precision, recall, F1-score, dan confusion matrix.

### Perbandingan Sebelum dan Sesudah Fine-Tuning

| Tahap | Test Accuracy | Test Loss | Macro F1-Score |
|---|---:|---:|---:|
| Transfer Learning (MobileNetV2 dibekukan) | 81,92% | 0,5330 | 0,83 |
| Setelah Fine-Tuning | **85,95%** | **0,4567** | **0,87** |

### Hasil Akhir (Setelah Fine-Tuning)

| Metrik | Nilai (Weighted Average) |
|---|---:|
| Accuracy | 85,95% |
| Precision | 86,14% |
| Recall | 85,95% |
| F1-Score | 85,94% |

### F1-Score per Kategori

| Kategori | Sebelum | Sesudah |
|---|---:|---:|
| Cardboard | 0,85 | 0,86 |
| Food Organics | 0,88 | 0,90 |
| Glass | 0,82 | 0,88 |
| Metal | 0,81 | 0,84 |
| Miscellaneous Trash | 0,66 | 0,73 |
| Paper | 0,83 | 0,86 |
| Plastic | 0,76 | 0,84 |
| Textile Trash | 0,89 | 0,91 |
| Vegetation | 0,95 | 0,98 |

### Pembahasan

- Fine-tuning meningkatkan akurasi pengujian dari 81,92% menjadi 85,95% dan menurunkan test loss, dengan peningkatan F1-score pada seluruh kategori.
- Kategori dengan performa terbaik adalah **Vegetation** (F1 0,98) dan **Textile Trash** (F1 0,91), yang memiliki ciri visual lebih khas.
- Kategori dengan performa terendah adalah **Miscellaneous Trash** (F1 0,73), karena kelas ini mencakup beragam jenis sampah dengan tampilan visual yang bervariasi.
- Pada tahap fine-tuning, akurasi training mencapai sekitar 99%, sedangkan akurasi validasi sekitar 85%. Selisih ini menunjukkan adanya indikasi *overfitting*, sehingga model masih dapat ditingkatkan.

---

## 🌐 Aplikasi Web

Model akhir diimplementasikan dalam aplikasi web berbasis Streamlit. Pengguna dapat mengunggah gambar sampah (`jpg`, `jpeg`, atau `png`), kemudian aplikasi menampilkan kategori hasil klasifikasi, *confidence score*, dan grafik probabilitas untuk sembilan kategori.

### Menjalankan Aplikasi

```bash
pip install -r requirements.txt
streamlit run app.py
```

### Struktur File Aplikasi

| File | Keterangan |
|---|---|
| `app.py` | Kode aplikasi Streamlit |
| `requirements.txt` | Daftar library yang dibutuhkan |
| `waste_classifier.keras` | Model hasil fine-tuning |
| `class_names.json` | Daftar nama kategori sampah |

---

## 🚀 Saran Pengembangan

- Menambahkan augmentasi gambar untuk mengurangi *overfitting*.
- Menerapkan *class weight* untuk mengatasi ketidakseimbangan jumlah data antar kategori.
- Menambah data sampah yang diambil langsung dari lingkungan kampus agar model lebih sesuai dengan kondisi nyata.
- Mencoba arsitektur CNN lain sebagai pembanding.

---

## 📚 Kesimpulan

Penerapan Transfer Learning berbasis MobileNetV2 dengan TensorFlow berhasil mengklasifikasikan sembilan kategori sampah pada dataset RealWaste dengan akurasi **85,95%** setelah fine-tuning. Model dapat membedakan jenis sampah berdasarkan karakteristik visualnya, dengan kesalahan klasifikasi yang paling banyak terjadi pada kategori Miscellaneous Trash. Hasil klasifikasi dapat dimanfaatkan melalui aplikasi web untuk membantu proses pemilahan sampah di lingkungan kampus, sebagai dukungan terhadap SDG 12.
