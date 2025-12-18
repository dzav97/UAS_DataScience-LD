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
project/
│
├── data/                   # Dataset (tidak di-commit, download manual)
│
├── notebooks/              # Jupyter notebooks
│   └── ML_Project.ipynb
│
├── src/                    # Source code
│   
├── models/                 # Saved models
│   ├── model_baseline.pkl
│   ├── model_rf.pkl
│   └── model_cnn.h5
│
├── images/                 # Visualizations
│   └── r
│
├── requirements.txt        # Dependencies
├── .gitignore
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
| ... | ... |

---

# 4. 🔧 Data Preparation
- Cleaning (missing/duplicate/outliers)  
- Transformasi (encoding/scaling)  
- Splitting (train/val/test)  

---

# 5. 🤖 Modeling
- **Model 1 – Baseline:** [...]  
- **Model 2 – Advanced ML:** [...]  
- **Model 3 – Deep Learning:** [...]  

---

# 6. 🧪 Evaluation
**Metrik:** Accuracy / F1 / MAE / MSE (pilih sesuai tugas)

### Hasil Singkat
| Model | Score | Catatan |
|-------|--------|---------|
| Baseline | [...] | |
| Advanced | [...] | |
| Deep Learning | [...] | |

---

# 7. 🏁 Kesimpulan
- Model terbaik: [...]  
- Alasan: [...]  
- Insight penting: [...]  

---

# 8. 🔮 Future Work
- [ ] Tambah data  
- [ ] Tuning model  
- [ ] Coba arsitektur DL lain  
- [ ] Deployment  

---

# 9. 🔁 Reproducibility
Gunakan environment:
