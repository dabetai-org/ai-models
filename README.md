# dabetai — AI Models

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-1.3-F7931E?logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/XGBoost-1.6-orange" alt="XGBoost">
  <img src="https://img.shields.io/badge/PyTorch-2.x-EE4C2C?logo=pytorch&logoColor=white" alt="PyTorch">
</p>

<p align="center">
  <em>Machine learning pipelines for training, evaluating, and serializing predictive models for diabetic complications.</em>
</p>

<p align="center">
  <a href="https://github.com/dabetai-org/ai-models">Repository</a>
  ·
  <a href="https://github.com/dabetai-org/ai-models/issues">Report Bug</a>
  ·
  <a href="https://chrisssp.vercel.app/assets/docs/papers/Prevenci%C3%B3n-de-Riesgos-de-la-Diabetes-Mediante-una-Plataforma-Inteligente-de-Monitorizaci%C3%B3n-y-Predicci%C3%B3n-de-Complicaciones-con-Inteligencia-Artificial.pdf">Research Paper</a>
</p>

<p align="center">
  <a href="README.md">🇬🇧 English</a> · <a href="README.es.md">🇪🇸 Español</a>
</p>

---

## About dabetai

**dabetai** is a comprehensive preventive ecosystem for diabetes that predicts complications like retinopathy, nephropathy, neuropathy, and diabetic foot before they become irreversible.

This repository contains the **AI Models** — complete pipelines for training, evaluating, and serializing machine learning models focused on predicting:

- Diabetic retinopathy
- Diabetic nephropathy
- Diabetic neuropathy
- Diabetic foot

The models are based on clinical and biometric data from the IOBP2 study and are optimized with advanced techniques such as class balancing, hyperparameter tuning, and cross-validation.

### Ecosystem

| Component | Repository | Stack |
|-----------|-----------|-------|
| **Mobile App** | [dabetai-org/mobile-app](https://github.com/dabetai-org/mobile-app) | React Native 0.79, Expo 53, Tailwind CSS |
| **Web Portal** | [dabetai-org/web-app](https://github.com/dabetai-org/web-app) | Angular 19, Tailwind CSS |
| **Core API** | [dabetai-org/api](https://github.com/dabetai-org/api) | NestJS 11, PostgreSQL, Prisma |
| **AI Inference API** | [dabetai-org/ai-api](https://github.com/dabetai-org/ai-api) | FastAPI, Python 3.11, MongoDB |
| **AI Models** (this) | [dabetai-org/ai-models](https://github.com/dabetai-org/ai-models) | Python, scikit-learn, XGBoost, PyTorch |
| **Landing** | [dabetai-org/landing](https://github.com/dabetai-org/landing) | Astro, Tailwind CSS |

## Features

- **Modular Dataset Preparation** — Automated per-complication data pipelines
- **Multi-Algorithm Experimentation** — Logistic Regression, Random Forest, LightGBM, XGBoost, SVM, AdaBoost
- **Hyperparameter Optimization** — Grid Search for optimal model configuration
- **Model Serialization** — Export trained models for production deployment
- **Automatic Reporting** — ROC curves, confusion matrices, feature importance visualizations

## Quick Start

### Prerequisites

- Python 3.11+
- pip

### Setup

```bash
git clone https://github.com/dabetai-org/ai-models.git
cd ai-models
pip install -r requirements.txt
```

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

## Usage

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

### Required Data

Data is based on the **IOBP2 (In Control)** study. Place files in `data/raw/datatables/`. See [CITATION.md](CITATION.md) for attribution and responsible use.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for branch naming, commit conventions, and PR workflow.

## License

This project is licensed under the GNU General Public License v3.0 — see the [LICENSE](LICENSE) file for details.

## Acknowledgments

**Authors:**
- Cardenas Cabal Fermín
- Ortiz Pérez Alejandro — alex03ortizperez@gmail.com
- Serrano Puertos Jorge Christian — christian.serrano.puertos@gmail.com

**Advisors:**
- Guarneros Nolasco Luis Rolando
- Cruz Ramos Nancy Aracely

**Academic Support:**
- Universidad Tecnológica del Centro de Veracruz
