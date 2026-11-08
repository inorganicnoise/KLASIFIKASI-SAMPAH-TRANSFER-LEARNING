
# Project Deep Learning - SDGs 12 Konsumsi dan Produksi yang Bertanggung Jawab

## ♻️ Implementasi Transfer Learning Berbasis CNN untuk Klasifikasi Jenis Sampah di Lingkungan Kampus

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow?style=for-the-badge)

Proyek ini berkaitan dengan **SDG 12: Responsible Consumption and Production (Konsumsi dan Produksi yang Bertanggung Jawab)**.

SDG 12 menekankan pentingnya pola konsumsi dan produksi yang bertanggung jawab, termasuk pengurangan limbah serta peningkatan pengelolaan sampah.

Melalui penerapan teknologi Deep Learning, proyek ini diharapkan dapat mendukung proses identifikasi jenis sampah sebagai salah satu upaya untuk meningkatkan kesadaran dan efektivitas pemilahan sampah.

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

Pengembangan sistem menggunakan pendekatan **Transfer Learning** berbasis **Convolutional Neural Network (CNN)** dengan framework **TensorFlow**. Model *pre-trained* akan dimanfaatkan dan disesuaikan dengan dataset gambar sampah agar mampu melakukan klasifikasi secara otomatis.

Proyek ini berfokus pada pemanfaatan teknologi Artificial Intelligence (AI) untuk membantu proses identifikasi dan pemilahan sampah. Sistem yang dikembangkan diharapkan dapat menjadi salah satu solusi pendukung pengelolaan sampah yang lebih efektif, khususnya dalam konteks lingkungan perguruan tinggi.

## 🎯 Latar Belakang

Sampah merupakan salah satu permasalahan lingkungan yang masih sering dijumpai, termasuk di lingkungan perguruan tinggi. Berbagai aktivitas akademik dan kegiatan sehari-hari menghasilkan beragam jenis sampah, seperti plastik, kertas, kardus, kaca, logam, dan sampah organik.

Namun, proses pemilahan sampah masih menjadi tantangan karena kurangnya pengetahuan mengenai pengelompokan sampah berdasarkan jenis materialnya. Sampah yang tercampur dapat menyulitkan proses pengelolaan dan daur ulang.

Seiring perkembangan teknologi Artificial Intelligence, khususnya Deep Learning, klasifikasi citra dapat dimanfaatkan untuk membantu mengenali berbagai jenis sampah secara otomatis berdasarkan karakteristik visualnya.

Melalui proyek ini, diterapkan metode Transfer Learning berbasis CNN menggunakan TensorFlow untuk mengembangkan model yang mampu mengklasifikasikan jenis sampah berdasarkan gambar.

Diharapkan sistem ini dapat menjadi bentuk pemanfaatan teknologi AI dalam mendukung pengelolaan sampah serta meningkatkan kesadaran terhadap pentingnya pemilahan sampah di lingkungan kampus.

## 🎯 Tujuan Proyek

1. Mengimplementasikan metode Transfer Learning berbasis CNN untuk klasifikasi jenis sampah.
2. Mengembangkan model Deep Learning menggunakan TensorFlow.
3. Mengidentifikasi berbagai kategori sampah berdasarkan citra gambar.
4. Mengevaluasi performa model berdasarkan hasil pengujian.
5. Menerapkan teknologi Artificial Intelligence sebagai pendukung proses identifikasi dan pemilahan sampah.

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

Dataset RealWaste terdiri dari sembilan kategori sampah sebagai berikut:

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

---

## 🧠 Metode dan Teknologi

Proyek ini menggunakan pendekatan Transfer Learning berbasis Convolutional Neural Network (CNN).

### 1. Transfer Learning

Transfer Learning merupakan pendekatan pembelajaran mesin yang memanfaatkan pengetahuan dari model yang telah dilatih sebelumnya (*pre-trained model*) untuk menyelesaikan tugas baru.

Pendekatan ini digunakan agar proses pengembangan model klasifikasi sampah dapat memanfaatkan fitur visual yang telah dipelajari dari dataset sebelumnya.

### 2. Convolutional Neural Network (CNN)

CNN merupakan salah satu arsitektur Deep Learning yang banyak digunakan dalam pengolahan citra. CNN mampu mempelajari karakteristik visual gambar melalui proses ekstraksi fitur, seperti bentuk, tekstur, dan pola.

### 3. Model yang Digunakan

Model utama yang direncanakan adalah **MobileNetV2**.

MobileNetV2 merupakan arsitektur CNN yang dirancang agar lebih ringan dan efisien dalam pemrosesan citra. Model ini dipilih sebagai pendekatan Transfer Learning untuk mengembangkan sistem klasifikasi sampah.

### 🛠️ Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| Bahasa Pemrograman | Python |
| Framework Deep Learning | TensorFlow / Keras |
| Metode | Transfer Learning |
| Arsitektur CNN | MobileNetV2 |
| Pengembangan | Google Colab |
| Pengolahan Data | NumPy, Pillow |
| Visualisasi | Matplotlib |
| Evaluasi Model | Scikit-learn |
| Version Control | Git & GitHub |

---

## ⚙️ Tahapan Pengembangan

Pengembangan sistem dilakukan melalui beberapa tahapan berikut:

### 1. Pengumpulan Dataset
Mengumpulkan dataset gambar sampah RealWaste yang terdiri dari sembilan kategori berbeda.

### 2. Exploratory Data Analysis (EDA)
Melakukan eksplorasi dataset untuk memahami struktur data, jumlah gambar setiap kategori, serta distribusi kelas.

### 3. Preprocessing Data
Melakukan pengolahan awal terhadap gambar, meliputi:
- Resizing gambar.
- Normalisasi nilai piksel.
- Pemeriksaan data.
- Augmentasi gambar untuk menambah variasi data pelatihan.

### 4. Pembagian Dataset
Membagi dataset menjadi tiga bagian:
- Training Set: data untuk melatih model.
- Validation Set: data untuk memantau proses pelatihan.
- Testing Set: data untuk menguji performa akhir model.

### 5. Implementasi Transfer Learning
Menggunakan arsitektur MobileNetV2 yang telah dilatih sebelumnya, kemudian menyesuaikan lapisan klasifikasi dengan sembilan kategori sampah.

### 6. Training Model
Melakukan proses pelatihan menggunakan TensorFlow agar model dapat mempelajari karakteristik visual dari setiap kategori sampah.

### 7. Evaluasi Model
Mengukur performa model menggunakan beberapa metrik evaluasi untuk mengetahui kemampuan klasifikasinya.

### 8. Pengujian dan Prediksi
Melakukan pengujian menggunakan gambar sampah baru yang belum pernah digunakan dalam proses training untuk melihat kemampuan model dalam melakukan klasifikasi.

---

## 📊 Evaluasi Model

Performa model akan dievaluasi menggunakan beberapa metrik berikut:

| Metrik | Keterangan |
|---|---|
| Accuracy | Mengukur persentase prediksi yang benar dari seluruh data pengujian. |
| Precision | Mengukur ketepatan hasil prediksi pada setiap kategori. |
| Recall | Mengukur kemampuan model mengenali seluruh data pada setiap kategori. |
| F1-Score | Mengukur keseimbangan antara precision dan recall. |
| Confusion Matrix | Menampilkan perbandingan antara label sebenarnya dan hasil prediksi model. |

Hasil evaluasi akan digunakan untuk menganalisis kemampuan model dalam mengenali masing-masing kategori sampah, termasuk kategori yang berpotensi mengalami kesalahan klasifikasi.

---

Proses implementasi, pelatihan model, pengujian, dan evaluasi akan dilakukan secara bertahap. Hasil pengembangan akan diperbarui seiring dengan kemajuan pengerjaan proyek.
