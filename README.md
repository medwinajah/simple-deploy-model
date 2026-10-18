# 🌸 Simple Deploy Model — Streamlit ML App

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.45%2B-FF4B4B.svg)](https://streamlit.io/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.6%2B-F7931E.svg)](https://scikit-learn.org/)
[![GitHub Repo](https://img.shields.io/badge/GitHub-pompymandislian%2Fsimple--deploy--model-181717.svg?logo=github)](https://github.com/pompymandislian/simple-deploy-model)

Proyek ini mendemonstrasikan cara membuat dan mendeploy aplikasi Machine Learning interaktif berbasis web menggunakan **Streamlit**.

Repository ini memiliki 2 aplikasi utama:
1. **🌸 Iris Species Predictor (`sesi_6_iris_app.py`)**: Aplikasi prediksi spesies bunga Iris secara *real-time* dengan multi-model selection (Logistic Regression, Decision Tree, Random Forest, SVM), confidence score, dan chart probabilitas.
2. **🚀 Streamlit Basics (`sesi_6_streamlit_basics.py`)**: Panduan dan demo interaktif berbagai komponen UI dasar Streamlit (widget, formulir, plot, metrik, dan layout kolom).

---

## 📁 Struktur File

```text
simple-deploy-model/
├── README.md                   # Dokumentasi proyek
├── requirements.txt            # Daftar dependensi library
├── .gitignore                  # Filter file cache & lingkungan virtual
├── train_model.py              # Script otomatis latih & simpan model ML
├── sesi_6_iris_app.py          # Aplikasi web prediksi bunga Iris
├── sesi_6_streamlit_basics.py  # Aplikasi web demo dasar-dasar Streamlit
├── iris_feature_names.txt      # Metadata nama fitur input
├── iris_target_names.txt       # Metadata nama target label
├── iris_logistic_model.pkl     # Model: Logistic Regression
├── iris_tree_model.pkl         # Model: Decision Tree
├── iris_forest_model.pkl       # Model: Random Forest
└── iris_svm_model.pkl          # Model: SVM (Support Vector Machine)
```

---

## ⚡ Panduan Cepat (Step-by-Step)

Ikuti langkah-langkah di bawah ini untuk menjalankan proyek di komputer lokal:

### Step 1: Clone Repository
```bash
git clone https://github.com/pompymandislian/simple-deploy-model.git
cd simple-deploy-model
```

### Step 2: Buat & Aktifkan Virtual Environment (Opsional tapi disarankan)
- **macOS / Linux:**
  ```bash
  python3 -m venv venv
  source venv/bin/activate
  ```
- **Windows:**
  ```bash
  python -m venv venv
  venv\Scripts\activate
  ```

### Step 3: Install Dependensi
```bash
pip install -r requirements.txt
```

### Step 4: Siapkan Model ML & Metadata
Jalankan script ini satu kali untuk melatih dan menghasilkan file model `.pkl` serta metadata `.txt`:
```bash
python train_model.py
```
> *Jika file `.pkl` sudah ada di repositori, langkah ini opsional.*

### Step 5: Jalankan Aplikasi Streamlit

- **Menjalankan Aplikasi Prediksi Iris:**
  ```bash
  streamlit run sesi_6_iris_app.py
  ```
  Buka browser di: **`http://localhost:8501`**

- **Menjalankan Aplikasi Streamlit Basics:**
  ```bash
  streamlit run sesi_6_streamlit_basics.py
  ```
  Buka browser di: **`http://localhost:8501`**

- **Menjalankan Keduanya Bersamaan (di 2 terminal berbeda):**
  - Terminal 1: `streamlit run sesi_6_iris_app.py --server.port 8501`
  - Terminal 2: `streamlit run sesi_6_streamlit_basics.py --server.port 8502`

---

## 📤 Cara Push Update ke GitHub

Jika Anda melakukan perubahan dan ingin memperbarui repositori GitHub:

```bash
# 1. Cek status perubahan file
git status

# 2. Tambahkan semua file yang berubah
git add .

# 3. Buat pesan commit
git commit -m "Update: Streamlit apps and models"

# 4. Pastikan remote sudah terhubung ke repository Anda
git remote set-url origin https://github.com/pompymandislian/simple-deploy-model.git

# 5. Push ke GitHub
git branch -M main
git push -u origin main
```

---

## 🛠️ Tech Stack
- **Language:** Python
- **Web Framework:** [Streamlit](https://streamlit.io/)
- **Machine Learning:** [Scikit-Learn](https://scikit-learn.org/)
- **Model Storage:** [Joblib](https://joblib.readthedocs.io/)
- **Data & Visual:** [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/)

---

## 👤 Author
**Pompy Mandislian**
- GitHub: [@pompymandislian](https://github.com/pompymandislian)
- Repo: [simple-deploy-model](https://github.com/pompymandislian/simple-deploy-model)
