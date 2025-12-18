<<<<<<< HEAD
# 📘 Judul Proyek
*(Penerapan Metode Machine Learning untuk Klasifikasi Gangguan Hati Menggunakan Dataset Liver Disorders.)*

## 👤 Informasi
- **Nama:** [Diaz Azkha Varissa]  
- **Repo:** [https://github.com/dzav97/UAS_DataScience-LD.git]  
- **Video:** [https://drive.google.com/file/d/1RGMPrKfVwBvehbcUSm3CUcwDS40xHfQa/view?usp=drive_link]  

---

# 1. 🎯 Ringkasan Proyek
- Proyek ini membangun sistem klasifikasi gangguan hati berdasarkan data hasil tes darah pada Dataset Liver Disorders (BUPA). Tahapan meliputi data understanding & preparation (hapus duplikat, mapping label, scaling), membangun 3 model (Baseline, Advanced ML, Deep Learning), lalu mengevaluasi performa menggunakan metrik klasifikasi dan menentukan model terbaik.  

---

# 2. 📄 Problem & Goals
**Problem Statements:**  
- [1.	Dataset Liver Disorders berisi data numerik hasil tes darah dan konsumsi alkohol yang perlu dimanfaatkan untuk memprediksi label selector sebagai indikasi gangguan hati secara akurat.]  
- [2.	Dataset memiliki distribusi kelas yang tidak seimbang sehingga diperlukan proses preprocessing dan pemilihan model yang tepat agar performa klasifikasi tidak bias.]  
- [3.	Dibutuhkan perbandingan performa antara beberapa pendekatan model, mulai dari model sederhana hingga model yang lebih kompleks, untuk mengetahui metode terbaik dalam menyelesaikan permasalahan klasifikasi ini.]  
- [4.	Diperlukan model deep learning yang mampu mempelajari pola dan hubungan kompleks antar fitur numerik pada data tabular.] 

**Goals:**  
- [1.	Membangun model machine learning untuk mengklasifikasikan kondisi gangguan hati pada dataset Liver Disorders dengan performa yang baik.]  
- [2.	Mengukur dan membandingkan performa tiga pendekatan model, yaitu model baseline, model machine learning lanjutan, dan model deep learning.]  
- [3.	Menentukan model terbaik berdasarkan metrik evaluasi klasifikasi seperti accuracy, precision, recall, dan F1-score.]  
- [4.	Menghasilkan pipeline pemodelan yang reproducible, sehingga eksperimen dapat dijalankan kembali dengan hasil yang konsisten.] 

---
## 📁 Struktur Folder
```
UAS_DataScience-LD/
│
├── data/                        # Dataset
│   └── bupa.data  
├── notebooks/
│   └── UAS_LD.ipynb         # Notebook utama
│
├── models/                      # Model tersimpan
│   ├── logistic_regression_model.pkl
│   ├── random_forest_model.pkl
│   └── mlp_model.h5             # keras
│
├── images/                      # Visualisasi (EDA & grafik training)
│   ├── distribusi kelas.png
│   ├── histogram gammagt.png
│   ├── heatmap korelasi.png
│   ├── grafik accuracy epoch.png
│   └── grafik loss epoch.h5
├── src/
│   └── empty.txt
├── requirements.txt
├── Checklist Submit.md
├── Laporan UAS Data Science.pdf
└── README.md
```
---

# 3. 📊 Dataset
- **Sumber:** [https://archive.ics.uci.edu/dataset/60/liver+disorders]  
- **Jumlah Data:** [345]  
- **Tipe:** [Klasifikasi]  

### Fitur Utama
| Fitur | Deskripsi |
|------|-----------|
| mcv | Mean Corpuscular Volume |
| alkphos | Alkaline Phosphotase |
| sgpt | Alanine Aminotransferase |
| sgot | Aspartate Aminotransferase |
| gammagt | Gamma-Glutamyl Transpeptidase |
| drinks | Jumlah konsumsi alkohol per hari |
| selector | Target/label (dimapping menjadi 0 dan 1) |

---

# 4. 🔧 Data Preparation
- Cleaning: cek missing value, hapus data duplikat
- Transformasi: mapping label selector (1→0, 2→1) dan scaling fitur numerik dengan StandardScaler
- Splitting: train-test split (stratified) untuk menjaga proporsi kelas

---

# 5. 🤖 Modeling
- **Model 1 – Baseline:** [Logistic Regression]  
- **Model 2 – Advanced ML:** [Random Forest Classifier]  
- **Model 3 – Deep Learning:** [MLP (Neural Network)]  

---

# 6. 🧪 Evaluation
**Metrik:** Accuracy, Precision, Recall, F1-Score (+ waktu training)

### Hasil Singkat
| Model | accuracy | precision | recall | f1 | train_time_sec |
|-------|--------|---------|-------|--------|---------|
| Logistic Regression | [0.6957] | [0.7021] | [0.8250] | [0.7586] | [0.0270] | |
| Random Forest | [0.7391] | [0.7292] | [0.8750] | [0.7955] | [0.5745] |  |
| MLP (Deep Learning) | [0.7826] | [0.7660] | [0.9000] | [0.8276] | [4.6542] |  |

---

# 7. 🏁 Kesimpulan
- Model terbaik: [MLP (Deep Learning)]  
- Alasan: [memiliki akurasi & F1 tertinggi serta recall paling tinggi (paling baik menangkap kelas positif)]  
- Insight penting: [model kompleks (RF/MLP) unggul dibanding model linear (LR), namun membutuhkan waktu training lebih besar.]  

---

# 8. 🔮 Future Work
- **Mengumpulkan lebih banyak data**
Dataset Liver Disorders memiliki jumlah data yang relatif kecil, sehingga penambahan data dapat membantu meningkatkan kemampuan generalisasi model.
-	**Menambah variasi data**
Variasi data dari latar belakang pasien yang lebih beragam dapat membuat model lebih robust terhadap berbagai kondisi.
-	**Feature engineering lebih lanjut**
Pengembangan fitur baru, seperti rasio antar enzim hati atau transformasi fitur tertentu, berpotensi meningkatkan performa model.


---

# 9. 🔁 Reproducibility
1.  **Clone Repository:**
    ```bash
    git clone https://github.com/dzav97/UAS_DataScience-LD.git
    ```

2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Jalankan Notebook:**
    Buka `notebooks/UAS_LD.ipynb` menggunakan Jupyter Notebook atau Google Colab.

