# 🍊 Oranges or Grapefruit Classification using Decision Tree

## 📊 Dataset Information
- [Kaggle Link](https://www.kaggle.com/datasets/joshmcadams/oranges-vs-grapefruit)
- **Total entries**: 10,000
- **Label distribution**:
  - Orange: 5,000
  - Grapefruit: 5,000

### Features:
- `diameter` (float): Diameter of the fruit
- `weight` (float): Weight of the fruit
- `red`, `green`, `blue` (int): RGB color components

---

## 🛠️ Tahapan dan Langkah-langkah

### 1. Persiapan Data
- Import library: pandas, matplotlib, seaborn, sklearn
- Load dataset CSV dari Kaggle
- Tampilkan informasi dasar (jumlah data, jenis kolom, distribusi label)

### 2. Preprocessing
- Encode label `name` menjadi angka (misal: orange = 0, grapefruit = 1)
- Pisahkan fitur (`X`) dan target (`y`)
- Lakukan pembagian data menjadi training dan testing (80:20)

### 3. Training Model
- Gunakan `DecisionTreeClassifier` dari `sklearn`
- Latih model dengan data training

### 4. Evaluasi Model
- Prediksi hasil untuk data testing
- Hitung akurasi, precision, recall, f1-score
- Tampilkan confusion matrix

### 5. Visualisasi
- Plot feature importance
- Visualisasikan decision tree lengkap

---

## 🧠 Model

- **Algorithm**: Decision Tree Classifier
- **Accuracy**: 94.35%
- **Evaluation**:
  - Precision, Recall, and F1-score above 0.93
  - Balanced performance on both classes

---

## 📌 Feature Importance

Berdasarkan hasil training, fitur paling berpengaruh adalah:

1. `diameter` ➜ Kontribusi tertinggi
2. `weight`, `green`, `red`, `blue` ➜ Kontribusi minor

---

## 🌳 Decision Tree Visualization

Struktur pohon keputusan menunjukkan bagaimana model melakukan split berdasarkan diameter dan fitur lainnya untuk menentukan klasifikasi.

![dt](https://github.com/user-attachments/assets/3b7638c4-6ed2-48eb-911a-183bea8d12b1)

---

## 💡 Conclusion

Model ini berhasil membedakan jeruk dan grapefruit dengan akurat menggunakan atribut fisik dan warna sederhana. Fitur `diameter` sangat dominan, menandakan bahwa ukuran merupakan pembeda utama antara kedua buah ini. Dengan akurasi sebesar **94.35%**, Decision Tree terbukti menjadi alat klasifikasi yang kuat dan mudah dipahami untuk data terstruktur.

---
