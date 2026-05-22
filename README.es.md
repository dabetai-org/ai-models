# dabetai — Modelos IA

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-1.3-F7931E?logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/XGBoost-1.6-orange" alt="XGBoost">
  <img src="https://img.shields.io/badge/PyTorch-2.x-EE4C2C?logo=pytorch&logoColor=white" alt="PyTorch">
</p>

<p align="center">
  <em>Pipelines de machine learning para entrenamiento, evaluación y serialización de modelos predictivos de complicaciones diabéticas.</em>
</p>

<p align="center">
  <a href="https://github.com/dabetai-org/ai-models">Repositorio</a>
  ·
  <a href="https://github.com/dabetai-org/ai-models/issues">Reportar Bug</a>
  ·
  <a href="https://chrisssp.vercel.app/assets/docs/papers/Prevenci%C3%B3n-de-Riesgos-de-la-Diabetes-Mediante-una-Plataforma-Inteligente-de-Monitorizaci%C3%B3n-y-Predicci%C3%B3n-de-Complicaciones-con-Inteligencia-Artificial.pdf">Artículo de Investigación</a>
</p>

<p align="center">
  <a href="README.md">🇬🇧 English</a> · <a href="README.es.md">🇪🇸 Español</a>
</p>

---

## Acerca de dabetai

**dabetai** es un ecosistema preventivo integral para la diabetes que predice complicaciones como retinopatía, nefropatía, neuropatía y pie diabético antes de que sean irreversibles.

Este repositorio contiene los **Modelos IA** — pipelines completos para entrenamiento, evaluación y serialización de modelos de machine learning enfocados en predecir:

- Retinopatía diabética
- Nefropatía diabética
- Neuropatía diabética
- Pie diabético

Los modelos se basan en datos clínicos y biométricos del estudio IOBP2 y están optimizados con técnicas avanzadas como balanceo de clases, optimización de hiperparámetros y validación cruzada.

### Ecosistema

| Componente | Repositorio | Stack |
|-----------|-----------|-------|
| **App Móvil** | [dabetai-org/mobile-app](https://github.com/dabetai-org/mobile-app) | React Native 0.79, Expo 53, Tailwind CSS |
| **Portal Web** | [dabetai-org/web-app](https://github.com/dabetai-org/web-app) | Angular 19, Tailwind CSS |
| **Core API** | [dabetai-org/api](https://github.com/dabetai-org/api) | NestJS 11, PostgreSQL, Prisma |
| **API de IA** | [dabetai-org/ai-api](https://github.com/dabetai-org/ai-api) | FastAPI, Python 3.11, MongoDB |
| **Modelos IA** (este) | [dabetai-org/ai-models](https://github.com/dabetai-org/ai-models) | Python, scikit-learn, XGBoost, PyTorch |
| **Landing** | [dabetai-org/landing](https://github.com/dabetai-org/landing) | Astro, Tailwind CSS |

## Funcionalidades

- **Preparación Modular de Datasets** — Pipelines automatizados por complicación
- **Experimentación Multi-Algoritmo** — Regresión Logística, Random Forest, LightGBM, XGBoost, SVM, AdaBoost
- **Optimización de Hiperparámetros** — Grid Search para configuración óptima
- **Serialización de Modelos** — Exportación de modelos entrenados para producción
- **Reportes Automáticos** — Curvas ROC, matrices de confusión, importancia de características

## Inicio rápido

### Prerrequisitos

- Python 3.11+
- pip

### Instalación

```bash
git clone https://github.com/dabetai-org/ai-models.git
cd ai-models
pip install -r requirements.txt
```

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

## Uso

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

### Datos requeridos

Los datos provienen del estudio **IOBP2 (In Control)**. Colocar los archivos en `data/raw/datatables/`. Ver [CITATION.md](CITATION.md) para atribución y uso responsable.

## Contribuciones

Por favor lee [CONTRIBUTING.md](CONTRIBUTING.md) para nuestras convenciones de ramas, commits y flujo de PRs.

## Licencia

Este proyecto está licenciado bajo GNU General Public License v3.0 — consulta el archivo [LICENSE](LICENSE) para más detalles.

## Reconocimientos

**Autores:**
- Cardenas Cabal Fermín
- Ortiz Pérez Alejandro — alex03ortizperez@gmail.com
- Serrano Puertos Jorge Christian — christian.serrano.puertos@gmail.com

**Asesores:**
- Guarneros Nolasco Luis Rolando
- Cruz Ramos Nancy Aracely

**Apoyo Académico:**
- Universidad Tecnológica del Centro de Veracruz
