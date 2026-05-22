# Dabetai AI Models — <span id="en3">EN</span> · <a href="#es_aim">ES</a>

Machine learning module with predictive models for type 1 diabetic complications, integrated into the Dabetai platform.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-1.3-blue?logo=scikitlearn" alt="scikit-learn">
  <img src="https://img.shields.io/badge/LightGBM-3.x-green?logo=lightgbm" alt="LightGBM">
  <img src="https://img.shields.io/badge/XGBoost-1.6-orange?logo=xgboost" alt="XGBoost">
  <img src="https://img.shields.io/badge/joblib-1.x-yellow" alt="joblib">
</p>

---

## What is Dabetai AI Models?

**Dabetai AI Models** contains the complete pipelines for training, evaluating, and serializing machine learning models focused on predicting:

- Diabetic retinopathy
- Diabetic nephropathy
- Diabetic neuropathy
- Diabetic foot

The models are based on clinical and biometric data from the IOBP2 study and are optimized with advanced techniques such as class balancing, hyperparameter tuning, and cross-validation.

---

## Features

- Modular and automated dataset preparation per complication
- Comparative experimentation with multiple algorithms (Logistic Regression, Random Forest, LightGBM, XGBoost, SVM, AdaBoost)
- Hyperparameter optimization via Grid Search
- Final model training and serialization
- Automatic report and visualization generation (ROC curves, confusion matrices, feature importance)

---

## Tech Stack

- **Python 3.11+**
- **scikit-learn**
- **LightGBM**
- **XGBoost**
- **joblib** for serialization
- **imbalanced-learn** for class balancing (SMOTE)
- **matplotlib** and **seaborn** for visualization

---

## Quick Start

### Prerequisites

- Python 3.11+
- pip

### Steps

```bash
git clone https://github.com/dabetai-org/ai-models.git
cd ai-models
pip install -r requirements.txt
```

---

## Project Structure

```
ai-models/
├── scripts/
│   ├── 01_prepare_datasets.py
│   ├── 02_run_experiments.py
│   └── 03_finalize_model.py
├── data/
│   ├── raw/
│   └── processed/
├── models/
├── reports/
│   └── figures/
└── requirements.txt
```

---

## Usage Guide

### 1. Prepare datasets

```bash
python scripts/01_prepare_datasets.py
```

### 2. Run experiments

```bash
python scripts/02_run_experiments.py
```

### 3. Finalize models

```bash
python scripts/03_finalize_model.py
```

---

## Required Data

Data is based on the **IOBP2 (In Control)** study. Place files in `data/raw/datatables/`. See [CITATION.md](CITATION.md) for attribution and responsible use.

---

## Ecosystem

| Repository | Purpose | Status |
|---|---|---|
| [mobile-app](https://github.com/dabetai-org/mobile-app) | Patient mobile app | Active |
| [web-app](https://github.com/dabetai-org/web-app) | Doctor web app | Active |
| [api](https://github.com/dabetai-org/api) | Main backend API | Active |
| [ai-api](https://github.com/dabetai-org/ai-api) | AI prediction API | Active |
| [ai-models](https://github.com/dabetai-org/ai-models) | ML models | Active |
| [landing](https://github.com/dabetai-org/landing) | Landing page | Active |

---

## Contributing

See [CONTRIBUTING.MD](CONTRIBUTING.MD).

---

## Acknowledgments

Developed by:

- Cardenas Cabal Fermín
- Ortiz Pérez Alejandro
- Serrano Puertos Jorge Christian

Advisors:

- Guarneros Nolasco Luis Rolando
- Cruz Ramos Nancy Aracely

Academic support:

- Universidad Tecnológica del Centro de Veracruz
