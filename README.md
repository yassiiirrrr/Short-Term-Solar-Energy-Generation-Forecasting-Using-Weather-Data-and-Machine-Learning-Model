# Short-Term Solar Energy Generation Forecasting Using Weather Data and Machine Learning

## 📝 Project Overview
Accurate forecasting of solar power generation is critical for integrating renewable energy into the grid, optimizing energy storage, and ensuring grid stability. This project develops a robust machine learning pipeline to predict short-term solar energy output based on weather conditions and plant telemetry data. 

Transitioning from traditional statistical methods, this project implements a progressive modeling approach—starting with optimized ensemble machine learning algorithms and scaling up to advanced deep learning architectures to capture complex, non-linear weather patterns.

## 🚀 Key Features
* **Automated Data Pipeline:** End-to-end data ingestion, cleaning, and feature engineering for multivariate weather and telemetry datasets.
* **Ensemble Baseline Models:** Highly optimized Random Forest and XGBoost regression models establishing a strong forecasting baseline.
* **Deep Learning Integration:** Advanced neural network architectures (TensorFlow/Keras) designed to capture deep temporal dependencies in weather variations.
* **Comprehensive Evaluation:** Rigorous performance benchmarking using industry-standard regression metrics.

## 🛠️ Technology Stack
* **Language:** Python 3.x
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn, XGBoost
* **Deep Learning:** TensorFlow, Keras
* **Development Environment:** Google Colab, Jupyter Notebooks

## 📂 Repository Structure
```text
├── data/                    # Dataset directory (Raw and Processed - excluded via .gitignore)
├── docs/                    # Architecture diagrams, design documents, and presentations
├── notebooks/               # Experimental Jupyter/Colab notebooks
│   ├── 01_EDA_and_Preprocessing.ipynb
│   ├── 02_Ensemble_Baselines_XGBoost_RF.ipynb
│   └── 03_Deep_Learning_Models.ipynb
├── src/                     # Modularized Python scripts for production
│   ├── data_loader.py       # Data ingestion and cleaning scripts
│   ├── feature_eng.py       # Feature selection and engineering
│   ├── model_trainer.py     # Training routines for ML and DL models
│   └── evaluate.py          # Metric calculations (R², RMSE, MAE)
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
