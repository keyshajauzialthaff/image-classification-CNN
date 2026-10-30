# Image-Classification-CNN

# Klasifikasi Karakter Kartun (Homer vs Bart Simpson) Menggunakan Convolutional Neural Network (CNN)

Repositori ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) Mata Kuliah **Analisis Data Tidak Terstruktur**. Proyek ini mengimplementasikan *Deep Learning* menggunakan arsitektur **Convolutional Neural Network (CNN)** dengan pustaka TensorFlow/Keras untuk mengklasifikasikan gambar karakter kartun antara Homer Simpson dan Bart Simpson.

## Tahapan Pengerjaan Proyek
Berdasarkan ketentuan tugas, proyek ini melalui tahapan-tahapan berikut:
1. **Import Library & Membaca Gambar:** Memuat pustaka pendukung dan membaca sampel citra dari direktori dataset.
2. **Data Splitting & Augmentasi:** Membagi data menjadi data *training* dan *testing*, serta menerapkan augmentasi data (*rescaling, rotation, zoom, horizontal flip*) untuk memperkaya variasi model.
3. **Pembangunan Model CNN:** 
   * *Feature Detector* menggunakan layer konvolusi (`Conv2D`).
   * *Pooling* menggunakan `MaxPooling2D` untuk mereduksi dimensi.
   * *Flattening* mengubah matriks fitur menjadi vektor 1D.
   * *Dense Neural Network* sebagai *hidden layer* (aktivasi ReLU) dan *output layer* (aktivasi Softmax).
4. **Evaluasi Model:** Menguji performa model menggunakan data *testing* dan menghasilkan laporan evaluasi berupa *Confusion Matrix*, *Akurasi* (~90.74%), serta *Classification Report*.
5. **Prediksi Gambar Tunggal & Menyimpan Model:** Menguji model untuk memprediksi satu gambar baru secara spesifik serta menyimpan bobot model (`.hdf5` dan `.json`).

---

## Libraries
* **Python**
* **TensorFlow**
* **OpenCV**
* **Scikit-Learn**
* **Matplotlib & Seaborn**

---

## 📁 Struktur File di Repository
```text
├── UAS ADTT.pdf                 # Laporan lengkap tugas akhir[cite: 1]
├── notebook_cnn_simpsons.ipynb  # Jupyter Notebook / Script Google Colab[cite: 3]
└── README.md                    # Dokumentasi repositori
