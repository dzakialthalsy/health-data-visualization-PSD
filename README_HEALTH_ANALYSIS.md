# 🏥 Health Data Exploration - Heart Disease Analysis

## 📋 Deskripsi

Notebook ini melakukan **Exploratory Data Analysis (EDA)** pada dataset penyakit jantung dari Kaggle dengan berbagai visualisasi untuk memahami pola dan faktor risiko penyakit jantung.

## 📊 Dataset

**Nama**: Heart Disease UCI  
**Sumber**: Kaggle  
**Link**: https://www.kaggle.com/datasets/ronitf/heart-disease-uci

### Kolom Dataset:

| Kolom | Deskripsi | Tipe |
|-------|-----------|------|
| `age` | Usia (tahun) | Numerik |
| `sex` | Jenis Kelamin (1 = Male, 0 = Female) | Kategorik |
| `cp` | Chest Pain Type (0-3) | Kategorik |
| `trestbps` | Tekanan Darah Saat Istirahat (mm Hg) | Numerik |
| `chol` | Kolesterol Serum (mg/dl) | Numerik |
| `fbs` | Gula Darah Puasa > 120 mg/dl (1 = True, 0 = False) | Kategorik |
| `restecg` | Hasil EKG Saat Istirahat (0-2) | Kategorik |
| `thalach` | Denyut Jantung Maksimum | Numerik |
| `exang` | Angina Akibat Olahraga (1 = Yes, 0 = No) | Kategorik |
| `oldpeak` | Depresi ST Akibat Olahraga | Numerik |
| `slope` | Kemiringan Segmen ST Exercise (0-2) | Kategorik |
| `ca` | Jumlah Pembuluh Darah Utama (0-3) | Numerik |
| `thal` | Thalassemia (0-3) | Kategorik |
| `target` | Target (1 = Penyakit Jantung, 0 = Tidak) | Target |

## 🚀 Cara Menggunakan

### 1. Download Dataset

```bash
# Kunjungi link berikut dan download heart.csv
https://www.kaggle.com/datasets/ronitf/heart-disease-uci
```

Atau gunakan Kaggle API:

```bash
kaggle datasets download -d ronitf/heart-disease-uci
unzip heart-disease-uci.zip
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Jalankan Notebook

```bash
# Opsi 1: Jupyter Notebook
jupyter notebook health_data_exploration.ipynb

# Opsi 2: Jupyter Lab
jupyter lab health_data_exploration.ipynb

# Opsi 3: VS Code
# Buka file .ipynb di VS Code dan jalankan sel per sel
```

### 4. Pastikan File Dataset

Pastikan file `heart.csv` berada di direktori yang sama dengan notebook, atau update path di sel 2:

```python
df = pd.read_csv('heart.csv')  # Update path jika perlu
```

## 📈 Visualisasi yang Tersedia

1. **Distribusi Target Variable** - Pie chart & bar chart
2. **Distribusi Usia & Jenis Kelamin** - Histogram, boxplot, pie chart
3. **Scatter Plot** - Kolesterol vs Denyut Jantung, Usia vs Tekanan Darah
4. **Chest Pain Type Analysis** - Bar chart & stacked bar
5. **Correlation Heatmap** - Heatmap korelasi antar fitur
6. **Pair Plot** - Matrix scatter plot fitur penting
7. **Box Plot** - Distribusi fitur numerik per target
8. **Risk Score Analysis** - Feature engineering & analisis
9. **Dashboard** - Comprehensive visualization dashboard

## 💡 Insight Utama

Setelah menjalankan analisis, Anda akan menemukan:

- **Faktor risiko utama** berdasarkan korelasi dengan target
- **Demografi pasien** (usia, jenis kelamin)
- **Prevalensi penyakit** per kategori
- **Pola hubungan** antar variabel kesehatan
- **Rekomendasi** untuk pencegahan dan screening

## 📁 Struktur File

```
workspace/
├── health_data_exploration.ipynb    # Notebook utama
├── heart.csv                         # Dataset (download terpisah)
└── README_HEALTH_ANALYSIS.md         # Dokumentasi ini
```

## 🎯 Tujuan Pembelajaran

Setelah menyelesaikan notebook ini, Anda akan memahami:

1. ✅ Cara melakukan EDA pada dataset kesehatan
2. ✅ Teknik visualisasi data dengan matplotlib & seaborn
3. ✅ Interpretasi korelasi dan pola data
4. ✅ Feature engineering sederhana (risk score)
5. ✅ Cara menyajikan insight dari data

## ⚠️ Catatan

- Dataset ini untuk tujuan edukasi dan penelitian
- Selalu konsultasikan dengan profesional medis untuk diagnosa
- Hasil analisis tidak menggantikan saran medis profesional

## 📚 Referensi

- [Kaggle Dataset](https://www.kaggle.com/datasets/ronitf/heart-disease-uci)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+disease)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)

---

**Selamat menganalisis! 🎉**
