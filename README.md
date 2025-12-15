# 🐶🐱 Dog vs Cat Classification with CNN

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk membangun model **Convolutional Neural Network (CNN)** menggunakan **TensorFlow/Keras** untuk mengklasifikasikan gambar **anjing vs kucing**. Dataset yang digunakan adalah dataset publik dari FreeCodeCamp.

---

## ⚙️ Langkah-langkah Utama

- **Install & Import Library**
  - TensorFlow, Keras (Sequential, Conv2D, MaxPooling2D, Flatten, Dense, Dropout)
  - ImageDataGenerator untuk augmentasi data
  - Numpy, Matplotlib untuk analisis & visualisasi

- **Dataset Preparation**
  - Dataset diunduh otomatis via `wget` dan diekstrak.
  - Struktur folder: `train/`, `validation/`, `test/` dengan subfolder `cats/` dan `dogs/`.
  - Hitung jumlah file untuk memastikan distribusi data.

- **Preprocessing**
  - Image resizing ke ukuran **150x150 px**.
  - Batch size: **128**.
  - Epochs: **15**.
  - Augmentasi data: rescale, rotation, zoom, horizontal flip.

- **Model Architecture (CNN)**
  - Conv2D + MaxPooling (beberapa lapisan)
  - Flatten
  - Dense (fully connected)
  - Dropout untuk regularisasi
  - Output layer dengan aktivasi sigmoid (binary classification)

- **Training**
  - Optimizer: Adam
  - Loss function: Binary Crossentropy
  - Metrics: Accuracy
  - Training dilakukan dengan data generator (train & validation).

- **Evaluation**
  - Model diuji pada dataset `test/`.
  - Visualisasi akurasi dan loss per epoch menggunakan Matplotlib.

---

## 📊 Hasil
- Model mampu membedakan gambar **anjing vs kucing** dengan akurasi yang cukup tinggi.
- Grafik training menunjukkan perbaikan akurasi seiring bertambahnya epoch.

---

## 🚀 Cara Menjalankan
1. Clone repository ini.
2. Jalankan notebook di Google Colab atau Jupyter Notebook.
3. Pastikan TensorFlow sudah terinstall.
4. Notebook akan otomatis mengunduh dataset dan melakukan training.
