<div align="center">

# Md Huzaifa Ansari

### Machine Learning Engineer • Systems & Production ML
**Bachelor in Computer Science @ Indian Institute of Technology Patna | CPI: 9.62**

[![Kaggle Notebooks Expert](https://img.shields.io/badge/Kaggle_Notebooks_Expert-Rank_%23752_(Top_1.25%25)-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/neurocipher)
[![Kaggle Datasets Expert](https://img.shields.io/badge/Kaggle_Datasets_Expert-Rank_%23185_(Top_0.3%25)-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/neurocipher)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/md-huzaifa-ansari/)
[![GitHub Stars](https://img.shields.io/badge/GitHub-Repositories-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)

<br>

[![Architecture](https://img.shields.io/badge/Architecture-Decoupled_Microservices-0052CC?style=flat-square)](#)
[![Latency SLA](https://img.shields.io/badge/Inference_SLA-Sub--10ms_FastAPI-blueviolet?style=flat-square)](#)
[![Deployment](https://img.shields.io/badge/Deployment-Containerized_Docker-0db7ed?style=flat-square&logo=docker&logoColor=white)](#)
[![Optimization](https://img.shields.io/badge/Optimization-Convex_KKT_%26_Vectorized_Ops-success?style=flat-square)](#)

</div>

---

### 🏛️ Core Engineering & Systems Focus

* **Enterprise Anomaly & Fraud Intelligence:** Architected **AegisCore**, an enterprise-grade fraud intelligence platform leveraging a decoupled **FastAPI** REST microservice architecture, **Docker** containerization, and automated **SMOTE** class rebalancing. Engineered for **sub-10ms inference latency** with persistent, thread-safe transaction logging to **SQLite**.
* **Generative Imputation Frameworks:** Developed scalable deep generative pipelines in **PyTorch** and **TensorFlow** implementing **Generative Adversarial Imputation Networks (GAIN)** for high-dimensional tabular data. Formulated custom minimax objective functions $V(G, D)$, partial missingness hint matrices $H$, and automated Bayesian hyperparameter tuning with **Optuna**.
* **High-Performance Algorithmic Engineering:** Derived and implemented statistical machine learning models strictly from first principles using pure Python and **C-contiguous NumPy arrays**. Formulated Support Vector Machine (SVM) dual representations using Lagrange multipliers, solved via convex **Quadratic Programming (QP)** with explicit verification of **Karush-Kuhn-Tucker (KKT)** boundary conditions.
* **Low-Level Array Systems & Memory:** Researched and profiled high-throughput tensor computing mechanics, analyzing **C-order vs. Fortran-order** memory layouts, N-dimensional strides, zero-copy pointer transformations, and SIMD/BLAS cache locality to maximize numerical execution speed.

---

### ⚙️ AegisCore: Microservice & Inference Architecture

```text
┌────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│                              AEGISCORE CONTAINERIZED INFERENCE RUNTIME                                 │
└────────────────────────────────────────────────────────────────────────────────────────────────────────┘
                                                    │
                                                    ▼
┌──────────────────────┐             ┌──────────────────────────────┐
│   CLIENT DASHBOARD   │ ──(HTTP)──> │      REST API (FASTAPI)      │
│  • Transaction Event │             │  • Asynchronous ASGI Workers │
│  • Batch Ingestion   │             │  • Strict Pydantic Schema    │
└──────────────────────┘             └──────────────────────────────┘
                                                    │
                                                    ▼
┌──────────────────────┐             ┌──────────────────────────────┐
│ TRANSACTION LOGGING  │ <──(Async)─ │   ML INFERENCE ENGINE        │
│  • SQLite Persistence│             │  • Serialized Artifact (.pkl)│
│  • Real-Time Auditing│             │  • SMOTE Balanced Pipeline   │
│  • Fraud Telemetry   │             │  • Sub-10ms Execution SLA    │
└──────────────────────┘             └──────────────────────────────┘
```

---

### 📦 Featured Production Repositories

| Repository Name | MLE Architecture & Systems Focus | Tech Stack | Production Status |
| :--- | :--- | :--- | :--- |
| **[`aegiscore-fraud-detection`](https://github.com/)** | **Enterprise Fraud Intelligence Platform**<br>• Decoupled microservice architecture with low-latency REST endpoints<br>• Synthetic Minority Over-sampling Technique (SMOTE) pipeline<br>• Serialized inference engine (`.pkl`) with async SQLite transaction logging | `Python 3.10`<br>`FastAPI`<br>`Docker`<br>`SMOTE`<br>`SQLite` | ![Production](https://img.shields.io/badge/Deployment-Dockerized-0db7ed?style=flat-square)<br>`Sub-10ms Latency`<br>`Microservice` |
| **[`gain-tabular-imputation`](https://github.com/)** | **Generative Adversarial Imputation Engine**<br>• Implements minimax loss $V(G, D)$ with Hint matrix $H$ conditioning<br>• Reconstruction of high-dimensional non-random tabular missingness<br>• Automated hyperparameter convergence optimization via Optuna | `PyTorch`<br>`TensorFlow`<br>`Optuna`<br>`NumPy`<br>`SciPy` | ![Package](https://img.shields.io/badge/Distribution-Pip_Installable-3776AB?style=flat-square&logo=pypi&logoColor=white)<br>`Production-Grade`<br>`PyPI Ready` |
| **[`svm-from-scratch-py`](https://github.com/)** | **Dual Convex Optimization Engine**<br>• Vectorized dual Lagrangian formulation solved via quadratic programming<br>• Explicit verification of KKT stationarity, primal, and dual feasibility<br>• Pure algorithmic implementation without high-level ML dependencies | `Python`<br>`NumPy (C-Contiguous)`<br>`SciPy (QP)`<br>`Matplotlib` | ![Algorithmic](https://img.shields.io/badge/Verification-KKT_Validated-success?style=flat-square)<br>`First Principles`<br>`Zero-Dep Core` |
| **[`numpy-internals-guide`](https://github.com/)** | **Low-Level Memory & Vectorization Mechanics**<br>• Systems-level profiling of C vs. Fortran memory contiguity and strides<br>• Zero-copy array slicing, broadcasting mechanics, and cache locality<br>• Benchmark suite for optimizing vectorized matrix operations | `C-Python API`<br>`NumPy Internals`<br>`Memory Profiler`<br>`BLAS` | ![Technical Spec](https://img.shields.io/badge/Specification-Open_Source-9cf?style=flat-square)<br>`Systems Guide`<br>`Benchmarked` |

---

### 📊 Competitive Machine Learning & Research Credentials

<div align="center">

| Track | Global Standing | Volume & Recognitions | Engineering Impact |
| :--- | :---: | :---: | :--- |
| **Kaggle Notebooks** | **Rank #752**<br>*(Top 1.25% Globally)* | **16 Medals**<br>30 Public Production Notebooks | End-to-end predictive pipelines, leakage-free cross-validation architectures, and production exploratory algorithms. |
| **Kaggle Datasets** | **Rank #185**<br>*(Top 0.3% Globally)* | **2 Medals**<br>3 Curated Datasets | High-utility tabular datasets built with schema constraints, zero data leakage, and rigorous statistical metadata. |
| **Community Engagement** | **Global Contributor**<br>*(NeuroCipher)* | **640+ Upvotes**<br>540+ Forks | Consistently utilized by practitioners for machine learning baselines, numerical foundations, and pipeline design. |

</div>

---

### 🛠️ Production Stack & Systems Taxonomy

```text
  [Core Languages]      Python (AsyncIO, CPython), C++, SQL, Bash
  [Machine Learning]    PyTorch, TensorFlow, Scikit-learn, XGBoost, LightGBM, Imbalanced-Learn (SMOTE)
  [Systems & Serving]   FastAPI, Uvicorn (ASGI), Docker, REST APIs, SQLite, ONNX Runtime
  [Optimization & Math] SciPy (Convex QP / Dual Lagrange), Optuna (Bayesian Search), NumPy (Striding / BLAS)
  [Software Standards]  Git, GitHub Actions CI/CD, Modular OOP, Unit Testing, Pydantic Schema Enforcement
```

---

<div align="center">

[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/md-huzaifa-ansari/)
[![Kaggle Badge](https://img.shields.io/badge/Kaggle-Profile-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/neurocipher)
[![GitHub Repositories](https://img.shields.io/badge/GitHub-Repositories-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)

</div>
