# Ujian Akhir Semester - Praktikum Pembelajaran Mesin

---
**Perbandingan Kinerja Arsitektur CNN: Studi Kasus pada LeNet-5, AlexNet, dan ResNet-50 Menggunakan Dataset CIFAR-10**
---

- Onixa Shafa Putri Wibowo - 1227050107
- Silvia Febriani - 1227050126
- Siti Nurbayanah - 1227050128

---

Repositori ini berisi implementasi dan analisis dari penelitian perbandingan tiga arsitektur Convolutional Neural Network (CNN), yaitu LeNet-5, AlexNet, dan ResNet-50. Evaluasi dilakukan dengan menggunakan dataset CIFAR-10 untuk menilai performa klasifikasi citra berdasarkan akurasi global, akurasi per kelas, dan loss pelatihan.

## 🎯 Tujuan Penelitian

* Membandingkan akurasi klasifikasi dari tiga arsitektur CNN yang berbeda kompleksitas
* Menganalisis kemampuan generalisasi dan efisiensi pelatihan tiap model
* Memberikan rekomendasi model berdasarkan kebutuhan dan kompleksitas data

## 🗃️ Dataset

* CIFAR-10
* 10 kelas (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
* Ukuran gambar: 32x32 piksel, berwarna (RGB)
* 50.000 gambar pelatihan dan 10.000 gambar pengujian

## 🧱 Arsitektur yang Digunakan

* LeNet-5: arsitektur CNN sederhana
* AlexNet: arsitektur lebih dalam dengan ReLU dan dropout
* ResNet-50: arsitektur deep CNN dengan residual connection

## 📊 Ringkasan Hasil

| Model     | Akurasi Global (%) | Loss Akhir |
| --------- | ------------------ | ---------- |
| LeNet-5   | 63.73              | 0.8267     |
| AlexNet   | 73.71              | 0.6340     |
| ResNet-50 | 91.56              | 0.7196     |

* ResNet-50 menunjukkan performa tertinggi dan akurasi yang merata di semua kelas.
* AlexNet memberikan hasil yang lebih baik dibanding LeNet-5, namun masih kesulitan pada kelas yang mirip secara visual.
* LeNet-5 cocok untuk tugas sederhana, namun kurang optimal untuk CIFAR-10.

## 🚀 Cara Menjalankan

1. Clone repositori:
   git clone https://github.com/SitiNurbayanah/UAS_PrakPM

2. Masuk ke direktori:
   cd UAS_PrakPM

3. Jalankan pelatihan model:
   python train\_lenet.py
   python train\_alexnet.py
   python train\_resnet50.py
