# 🚀 Machine Learning Project: Clustering & Classification (BMLP Submission)

## 📌 Overview
Project ini merupakan submission akhir dari kelas Machine Learning di Dicoding, yang bertujuan untuk mengintegrasikan teknik **unsupervised learning (clustering)** dan **supervised learning (classification)** dalam satu pipeline end-to-end.

Pada tahap awal, dilakukan clustering untuk menghasilkan label (Target) dari dataset tanpa label. Selanjutnya, label tersebut digunakan untuk membangun model klasifikasi yang mampu memprediksi kelas berdasarkan fitur yang tersedia.

---

## 🎯 Objectives
- Mengelompokkan data transaksi menggunakan algoritma clustering
- Menghasilkan label baru dari hasil clustering
- Membangun model klasifikasi untuk memprediksi label tersebut
- Mengevaluasi performa model menggunakan berbagai metrik

---

## 📊 Dataset
Dataset yang digunakan merupakan hasil modifikasi dari:
- **Bank Transaction Dataset for Fraud Detection (Kaggle)**
- Versi: Google Drive (Dicoding Submission)

Karakteristik dataset:
- Data transaksi keuangan
- Terdiri dari fitur numerik dan kategorikal
- Tidak memiliki label awal (unsupervised)

---

## ⚙️ Technologies & Tools
- Python
- Pandas & NumPy
- Scikit-learn (v1.7.0)
- Matplotlib & Seaborn
- Joblib

---

## 🔄 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Menampilkan data (`head`, `info`, `describe`)
- Analisis distribusi data
- Korelasi antar fitur
- Visualisasi histogram

### 2. Data Preprocessing
- Handling missing values (`dropna`)
- Removing duplicates
- Drop kolom tidak relevan (ID, Address, Date)
- Encoding fitur kategorikal (LabelEncoder)
- Handling outliers
- Feature scaling (StandardScaler)
- Feature binning (opsional advanced)

---

## 🧠 Clustering Model

### 📌 Algorithm
- K-Means Clustering

### 📊 Method
- Elbow Method untuk menentukan jumlah cluster optimal
- Silhouette Score untuk evaluasi cluster

### 🔍 Additional (Advanced)
- PCA (Principal Component Analysis) untuk reduksi dimensi

### 💾 Model Output
- `model_clustering.h5`
- `PCA_model_clustering.h5` (opsional)

---

## 📈 Clustering Results
- Dataset berhasil dikelompokkan menjadi beberapa cluster
- Setiap cluster memiliki karakteristik unik berdasarkan fitur transaksi

Contoh insight:
- Cluster tertentu menunjukkan pola transaksi dengan nilai tinggi
- Cluster lain menunjukkan aktivitas transaksi rendah

---

## 🧾 Data Output
- Dataset hasil clustering: `data_clustering.csv`
- Dataset inverse transform: `data_clustering_inverse.csv` (opsional)
- Kolom target hasil clustering: **Target**

---

## 🤖 Classification Model

### 📌 Algorithm
- Decision Tree (mandatory)
- [Tambahkan model lain jika ada, contoh: Random Forest]

### ⚙️ Process
- Train-test split
- Model training
- Model evaluation

### 📊 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score

### 🔧 Advanced
- Hyperparameter tuning untuk meningkatkan performa model

### 💾 Model Output
- `decision_tree_model.h5`
- `explore_<model>_classification.h5` (opsional)
- `tuning_classification.h5` (opsional)

---

## 📈 Classification Results
Model klasifikasi mampu memprediksi label hasil clustering dengan performa yang baik berdasarkan metrik evaluasi.

---

## 🚀 How to Run

1. Clone repository:
```bash
git clone https://github.com/username/nama-repo.git

2. Masuk ke folder project:
cd nama-repo

3. Install dependencies:
pip install -r requirements.txt

4. Jalankan notebook:
jupyter notebook

