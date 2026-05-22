<a href="#en3"><span id="es_aim">ES</span></a> · <a href="#en3">EN</a>

# Dabetai AI Models

Módulo de machine learning con modelos predictivos para complicaciones diabéticas tipo 1, integrados en la plataforma Dabetai.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-1.3-blue?logo=scikitlearn" alt="scikit-learn">
  <img src="https://img.shields.io/badge/LightGBM-3.x-green?logo=lightgbm" alt="LightGBM">
  <img src="https://img.shields.io/badge/XGBoost-1.6-orange?logo=xgboost" alt="XGBoost">
  <img src="https://img.shields.io/badge/joblib-1.x-yellow" alt="joblib">
</p>

---

## ¿Qué es Dabetai AI Models?

**Dabetai AI Models** contiene los pipelines completos para entrenamiento, evaluación y serialización de modelos de machine learning enfocados en predecir:

- Retinopatía diabética
- Nefropatía diabética
- Neuropatía diabética
- Pie diabético

Los modelos se basan en datos clínicos y biométricos del estudio IOBP2 y están optimizados con técnicas avanzadas como balanceo de clases, optimización de hiperparámetros y validación cruzada.

---

## Funcionalidades

- Preparación modular y automatizada de datasets por complicación
- Experimentación comparativa con múltiples algoritmos (Regresión Logística, Random Forest, LightGBM, XGBoost, SVM, AdaBoost)
- Optimización de hiperparámetros mediante Grid Search
- Entrenamiento final y serialización de modelos
- Generación automática de reportes y visualizaciones (ROC, matrices de confusión, importancia de características)

---

## Tecnologías

- **Python 3.11+**
- **scikit-learn**
- **LightGBM**
- **XGBoost**
- **joblib** para serialización
- **imbalanced-learn** para balanceo de clases (SMOTE)
- **matplotlib** y **seaborn** para visualización

---

## Inicio rápido

### Prerrequisitos

- Python 3.11+
- pip

### Pasos

```bash
git clone https://github.com/dabetai-org/ai-models.git
cd ai-models
pip install -r requirements.txt
```

---

## Estructura del proyecto

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

## Guía de uso

### 1. Preparar datasets

```bash
python scripts/01_prepare_datasets.py
```

### 2. Ejecutar experimentos

```bash
python scripts/02_run_experiments.py
```

### 3. Finalizar modelos

```bash
python scripts/03_finalize_model.py
```

---

## Datos requeridos

Los datos provienen del estudio **IOBP2 (In Control)**. Colocar los archivos en `data/raw/datatables/`. Ver [CITATION.md](CITATION.md) para atribución y uso responsable.

---

## Ecosistema

| Repositorio | Propósito | Estado |
|---|---|---|
| [mobile-app](https://github.com/dabetai-org/mobile-app) | App para pacientes | Activo |
| [web-app](https://github.com/dabetai-org/web-app) | App web para médicos | Activo |
| [api](https://github.com/dabetai-org/api) | API principal del backend | Activo |
| [ai-api](https://github.com/dabetai-org/ai-api) | API de IA y predicciones | Activo |
| [ai-models](https://github.com/dabetai-org/ai-models) | Modelos de machine learning | Activo |
| [landing](https://github.com/dabetai-org/landing) | Página de aterrizaje | Activo |

---

## Contribuciones

Ver [CONTRIBUTING.MD](CONTRIBUTING.MD).

---

## Reconocimientos

Desarrollado por:

- Cardenas Cabal Fermín
- Ortiz Pérez Alejandro
- Serrano Puertos Jorge Christian

Asesores:

- Guarneros Nolasco Luis Rolando
- Cruz Ramos Nancy Aracely

Apoyo académico:

- Universidad Tecnológica del Centro de Veracruz
