# Phishing Website Detection Using Machine Learning

# 🛡️ Phishing Website Detection Application

A full-stack web application that uses Machine Learning to analyze and detect potential phishing URLs in real time. The project features an interactive front-end interface built with modern UI cards alongside a Flask backend, powered by custom scikit-learn models.

---

## 🚀 Features
* **Real-time URL Prediction:** Evaluates incoming URLs via pre-trained ML estimators.
* **Vectorized Feature Extraction:** Uses custom `vectorizer.pkl` pipelines to process raw inputs.
* **Modern Premium Interface:** Beautifully designed dashboards featuring responsive elements and glassmorphic UI states.

---

## 🛠️ Tech Stack
* **Backend Framework:** Python / Flask
* **Machine Learning Library:** scikit-learn (v1.5.1 / v1.9.1 compatible)
* **Front-End Styling:** Tailwind CSS 
* **Model Serialization:** Pickle (`.pkl`)

---

## 📂 Repository Structure
```text
phishing_website/
│
├── app.py                 # Core Flask backend application
├── vectorizer.pkl         # Trained URL text feature extractor
├── phishing.pkl           # Saved classification model weights
├── .gitignore             # Git environment filter configuration
├── README.md              # Project usage documentation
│
└── templates/             # Server-side HTML render directory
    └── index.html         # Live user portal interface
```

---

## ⚙️ Installation & Local Setup

Follow these steps to run this application on your local machine:

### 1. Clone the Project
```bash
git clone https://github.com
cd phishing_website
```

### 2. Configure Your Virtual Environment
```bash
# Create environment
python -m venv env

# Activate environment (Windows PowerShell)
.\env\Scripts\Activate.ps1

# Activate environment (Mac/Linux)
source env/bin/activate
```

### 3. Install Required Packages
```bash
pip install flask scikit-learn numpy
```
*Note: If you run into model structural mismatch warnings, force-install the matching version using `pip install scikit-learn==1.5.1`.*

### 4. Boot Up the Server
```bash
python app.py
```
Open your browser and navigate to **`http://127.0.0.1:5000`** to interact with the system.
