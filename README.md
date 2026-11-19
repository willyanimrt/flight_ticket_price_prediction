# Flight Ticket Price Prediction

This project focuses on predicting flight ticket prices using Machine Learning techniques based on various flight characteristics, including airline, travel class, number of stops, route, flight duration, and days remaining before departure.

The project involves data exploration, data preprocessing, feature engineering, and regression modeling to identify patterns and estimate flight ticket prices.

A Streamlit-based web application was also developed to allow users to interactively input flight details and obtain estimated ticket prices.

# Key Features

- Exploratory Data Analysis (EDA)
- Data Cleaning & Preprocessing
- Feature Engineering
- Flight Ticket Price Prediction using Machine Learning
- Regression Model Evaluation
- Interactive Prediction Web App using Streamlit

# Tools & Technologies

- Python
- Pandas & NumPy
- Scikit-learn
- Matplotlib & Seaborn
- Streamlit
- Joblib

# Project Objective

To develop a Machine Learning model that estimates flight ticket prices based on flight characteristics and provides users with an interactive prediction experience.

## Isi folder

```text
airlines-streamlit-deployment/
  app.py
  requirements.txt
  models/
    best_flight_price_model.pkl
    route_info.pkl
```

## Cara menjalankan di VS Code

1. Open VS Code.
2. Choose `File > Open Folder...` after that open `airlines-streamlit-deployment`.
3. Open terminal VS Code.
4. Create virtual environment.

Disarankan memakai Python 3.11 atau 3.12 untuk kompatibilitas package machine learning:

```powershell
py -3.11 -m venv .venv
```

Jika hanya ada satu Python dan versinya sudah cocok, bisa pakai:

```bash
python -m venv .venv
```

5. Aktifkan virtual environment.

PowerShell Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

Command Prompt Windows:

```cmd
.venv\Scripts\activate.bat
```

6. Pastikan terminal sudah memakai virtual environment:

```powershell
python --version
where python
```

Path Python harus mengarah ke folder `.venv`.

7. Install dependency:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

8. Jalankan aplikasi:

```bash
python -m streamlit run app.py
```

9. Buka URL yang muncul di terminal, biasanya:

```text
http://localhost:8501
```

## Fitur input model

Model menerima kolom berikut:

- `airline`
- `departure_time`
- `stops`
- `arrival_time`
- `class`
- `duration`
- `days_left`
- `route`

## Catatan

Jika saat menjalankan app muncul error dependency saat membuka file `.pkl`, pastikan versi package di `requirements.txt` sudah ter-install di virtual environment yang aktif.

Lihat juga `TROUBLESHOOTING.md` jika muncul error `ModuleNotFoundError: No module named 'sklearn'`.
