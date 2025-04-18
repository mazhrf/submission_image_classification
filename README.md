# 🐾 Klasifikasi Gambar Kucing dan Anjing dengan Deep Learning

Proyek ini merupakan implementasi deep learning untuk mengklasifikasikan gambar menjadi dua kelas: **Kucing 🐱** dan **Anjing 🐶**. Model ini dilatih menggunakan Keras dan TensorFlow dengan dataset yang diproses melalui `ImageDataGenerator`.

## 📁 Struktur Proyek
submission_image_classification
├───tfjs_model
| ├───group1-shard1of3.bin
| ├───group1-shard2of3.bin
| ├───group1-shard3of3.bin
| └───model.json
├───tflite
| ├───model.tflite
| └───label.txt
├───saved_model
| ├───saved_model.pb
| ├───fingrprint.pb
| └───variables
├───notebook.ipynb
├───README.md
└───requirements.txt

## 🧠 Model

Model dibangun menggunakan TensorFlow Keras dengan arsitektur CNN dasar. Output model berupa sigmoid untuk klasifikasi biner (kucing vs anjing).

## 🏗️ Alur Kerja

1. **Persiapan Dataset**: Folder `train/`, `validation/`, dan `test/` masing-masing berisi subfolder `cats/` dan `dogs/`.
2. **Training Model**:
   - Menggunakan `ImageDataGenerator` untuk augmentasi.
   - Optimizer: Adam.
   - Loss Function: Binary Crossentropy.
3. **Evaluasi dan Visualisasi**:
   - Menampilkan grafik akurasi dan loss.
   - Membuat confusion matrix.
4. **Inference**:
   - Mengunggah gambar untuk prediksi.
   - Menampilkan hasil klasifikasi dan confidence.
