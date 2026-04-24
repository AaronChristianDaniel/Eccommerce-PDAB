# 🛒 E-Commerce Customer Churn Prediction

Prediksi churn pelanggan e-commerce menggunakan algoritma **K-Nearest Neighbors (KNN)**.

---

## 📌 Deskripsi

Churn pelanggan adalah kondisi di mana pelanggan berhenti menggunakan layanan atau tidak aktif melakukan transaksi. Proyek ini membangun model machine learning untuk mendeteksi pelanggan yang berpotensi churn berdasarkan data historis perilaku mereka.

Dengan model ini, bisnis dapat:
- Mengidentifikasi pelanggan berisiko lebih awal
- Mengambil tindakan preventif (promo, follow-up, peningkatan layanan)
- Mengurangi tingkat churn secara keseluruhan

---

## 📂 Struktur Proyek

```
├── data_ecommerce_customer_churn.csv   # Dataset
├── customer_churn_knn_fixed.ipynb      # Notebook utama
└── README.md
```

---

## 📊 Dataset

| Info | Detail |
|---|---|
| Jumlah Data | 3.941 baris |
| Jumlah Fitur | 10 fitur input |
| Target | `Churn` (0 = Tidak Churn, 1 = Churn) |
| Churn Rate | ~17% |

**Fitur yang digunakan:**

| Fitur | Deskripsi |
|---|---|
| `Tenure` | Lama menjadi pelanggan (bulan) |
| `WarehouseToHome` | Jarak gudang ke rumah pelanggan |
| `NumberOfDeviceRegistered` | Jumlah perangkat yang terdaftar |
| `PreferedOrderCat` | Kategori produk yang sering dipesan |
| `SatisfactionScore` | Skor kepuasan pelanggan (1–5) |
| `MaritalStatus` | Status pernikahan |
| `NumberOfAddress` | Jumlah alamat pengiriman tersimpan |
| `Complain` | Pernah mengajukan komplain (0/1) |
| `DaySinceLastOrder` | Hari sejak terakhir order |
| `CashbackAmount` | Total cashback yang diterima |

---

## ⚙️ Alur Pipeline

```
Load Data → EDA → Preprocessing → Oversampling → Split & Scale → Optimasi K → Training → Evaluasi
```

---

## 🚀 Cara Menjalankan

1. Clone repo ini:
```bash
git clone https://github.com/AaronChristianDaniel/Eccommerce-PDAB.git
cd Eccommerce-PDAB
```

2. Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Buka notebook di Jupyter atau upload ke Google Colab.

---

## 📈 Hasil

Model KNN dioptimasi dengan mencari nilai K terbaik (K=1–20), dievaluasi menggunakan accuracy, precision, recall, F1-score, dan confusion matrix.

---
---

## 👤 Author

**Aaron Christian Daniel**
