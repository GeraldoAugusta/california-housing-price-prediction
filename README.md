### Machine Learning Portfolio Project  
**Author:** Geraldo Augusta
**Email:** geraldonyoman14@gmail.com  
**LinkedIn:** https://linkedin.com/in/geraldoaugusta  
**GitHub:** https://github.com/geraldoaugusta  

# 🏡 California Housing Price Prediction
Proyek ini bertujuan untuk memprediksi harga rumah di California menggunakan teknik *Machine Learning Regression*. Dataset yang digunakan adalah **California Housing Dataset** dari scikit-learn.

Proyek ini mencakup tahapan lengkap Data Science:
- Exploratory Data Analysis (EDA)
- Preprocessing
- Model Training (Linear Regression & Random Forest)
- Model Evaluation
- Visualisasi Prediksi dan Feature Importance

---

## 📊 Dataset
Dataset berisi informasi mengenai kondisi demografi dan karakteristik wilayah di California, seperti:

- `MedInc` — Median income (pendapatan rata-rata)
- `HouseAge` — Umur rumah
- `AveRooms` — Rata-rata jumlah ruangan
- `AveOccup` — Rata-rata jumlah penghuni
- `Latitude` — Garis lintang
- `Longitude` — Garis bujur
- `MedHouseVal` — **Harga median rumah** (target)

Dataset berasal dari:
`sklearn.datasets.fetch_california_housing`

---

## 🔍 Exploratory Data Analysis (EDA)
Beberapa analisis yang dilakukan:

### ✔ Distribusi fitur  
Menggunakan histogram untuk melihat persebaran masing-masing variabel.

### ✔ Korelasi antar fitur  
Menggunakan heatmap untuk mengidentifikasi fitur yang paling memengaruhi harga rumah.

### ✔ Scatter plot  
Visualisasi hubungan antara tiap fitur dan nilai rumah.

---

## 🔧 Preprocessing
Tahap preprocessing meliputi:

- Memisahkan fitur (X) dan target (y)
- Train-test split (80:20)
- Scaling dengan StandardScaler untuk model linear
- Random Forest tidak memerlukan scaling

---

## 🤖 Modeling
Dua model yang digunakan:

### **1. Linear Regression (Baseline)**  
Model dasar untuk membandingkan performa awal.

### **2. Random Forest Regressor**  
Model berbasis ensemble yang biasanya menghasilkan performa lebih baik pada data non-linear.

---

## 📈 Evaluation Metrics

Metric evaluasi yang digunakan:

- **RMSE (Root Mean Squared Error)**
- **R² Score**

Contoh hasil evaluasi (mungkin berbeda di komputer Anda):

| Model | RMSE | R² |
|-------|-------|--------|
| Linear Regression | ~0.73 | ~0.60 |
| Random Forest | ~0.47 | ~0.82 |

> Random Forest memberikan performa yang jauh lebih baik.

---

## 📉 Visualizations

Visualisasi yang dibuat:

### ✔ Prediksi vs Aktual
Scatter plot nilai aktual dibandingkan nilai prediksi.

### ✔ Error Distribution  
Distribusi error untuk melihat apakah model bias.

### ✔ Feature Importance  
Menampilkan fitur apa yang paling berpengaruh terhadap harga rumah.
