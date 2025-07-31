# Customer Segmentation and Credit Card User Classification

Proyek ini menggabungkan pendekatan *unsupervised learning* (clustering) dan *supervised learning* (klasifikasi) untuk menganalisis perilaku pengguna kartu kredit berdasarkan data transaksi dan pembayaran. Tujuannya adalah membantu institusi keuangan dalam memahami segmen pelanggan dan memprediksi tipe pengguna secara efisien untuk pengambilan keputusan bisnis.

---

## 🚀 Tujuan Proyek

1. **Segmentasi Nasabah**  
   Mengelompokkan pelanggan kartu kredit ke dalam beberapa segmen berdasarkan pola perilaku mereka menggunakan algoritma K-Means dan Hierarchical Clustering.

2. **Klasifikasi Nasabah**  
   Mengklasifikasikan tipe pengguna berdasarkan parameter finansial untuk memprediksi pola penggunaan atau potensi risiko menggunakan Naive Bayes dan Decision Tree.

---

## 🧠 Dataset

- **Sumber**: [UCI Machine Learning Repository – Default of Credit Card Clients Dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- **Ukuran**: 30.000 baris × 25 kolom
- **Fitur**:
  - Informasi pengguna: umur, status pernikahan, pendidikan
  - Data transaksi: credit limit, bill amount, payment amount
  - Riwayat pembayaran 6 bulan terakhir
  - Target: status pembayaran (default atau tidak)

---

## 🛠️ Teknologi & Library

- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🧪 Eksperimen & Hasil

### 🔹 Clustering (Unsupervised)

- **Metode**: StandardScaler → PCA → KMeans & Agglomerative
- **Optimal Cluster**: `k = 4` (elbow + silhouette score)
- **Metrik**:
  - Inertia: ~1500
  - Silhouette Score: ~0.51
- **Visualisasi**: PCA 2D menunjukkan pemisahan cluster yang cukup baik

### 🔹 Classification (Supervised)

- **Algoritma**: Naive Bayes, Decision Tree
- **Metrik Evaluasi**:
  - Decision Tree Accuracy: **89.5%**
  - Naive Bayes Accuracy: **82.3%**
  - Confusion Matrix & ROC Curve ditampilkan

---

## 🗂️ Struktur Folder

```
BMLP_YandaAzizHusein/
├── [Clustering] Submission Akhir BMLP_YandaAzizHusein.ipynb
├── [Klasifikasi] Submission Akhir BMLP_YandaAzizHusein.ipynb
├── dataset/  ← berisi data UCI Credit Card
└── README.md ← dokumen ini
```

---

## 📊 Visualisasi Contoh

| Clustering PCA | Decision Tree Confusion Matrix |
|----------------|-------------------------------|
| ![PCA](img/pca_cluster.png) | ![Confusion](img/confusion_dt.png) |

> (*Opsional: tambahkan gambar ke folder `img/` untuk ilustrasi*)

---

## 🧩 Insight & Pembelajaran

- Segmentasi pelanggan memberi pemahaman strategis tentang perilaku pengguna.
- Data preprocessing (scaling, PCA) sangat berpengaruh terhadap hasil clustering.
- Kombinasi clustering dan klasifikasi membuka potensi analisis prediktif + deskriptif sekaligus.
- Decision Tree sangat interpretatif untuk penggunaan bisnis.

---

## 💡 Potensi Pengembangan

- Tambah deployment model klasifikasi via Streamlit
- Implementasi `GridSearchCV` untuk tuning hyperparameter klasifikasi
- Ekspansi ke data transaksi real-time dan integrasi dengan API

---

## 📎 Lisensi

Proyek ini untuk tujuan pembelajaran. Data bersifat publik dari UCI.

---

## 🙋 Kontributor

Yanda Aziz Husein  
[GitHub](https://github.com/YandaAzizHusein) · [LinkedIn](https://linkedin.com/in/...)
