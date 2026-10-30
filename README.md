# Short-Term Solar Energy Generation Forecasting Using Weather Data and Machine Learning

## 📝 Project Overview
Accurate forecasting of solar power generation is critical for integrating renewable energy into the grid, optimizing energy storage, and ensuring grid stability. This project develops a robust machine learning pipeline to predict short-term solar energy output based on weather conditions and plant telemetry data.

Transitioning from traditional statistical methods, this project implements a progressive modeling approach—starting with optimized ensemble machine learning algorithms and scaling to an interactive web deployment to bridge the gap between back-end data science and front-end utility management.

## 🚀 Key Features
- **Cyclic Feature Engineering:** Transforms standard chronological timestamps into cyclic trigonometric features (`hour_sin`, `month_cos`) to natively map continuous diurnal and seasonal solar patterns.
- **Ensemble Baseline Models:** Highly optimized Random Forest and XGBoost regression models establishing a strong forecasting baseline against non-linear weather shifts.
- **Live Prototype Deployment:** A fully functional Gradio web interface that processes real-time weather inputs and returns instantaneous active power predictions (kW).
- **Automated Data Pipeline:** End-to-end data ingestion, cleaning, and chronological 80/20 train-test splitting to prevent look-ahead bias.

## 🛠️ Technology Stack
- **Language:** Python 3.x
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, XGBoost
- **Web Deployment:** Gradio, Joblib
- **Development Environment:** Google Colab, Jupyter Notebooks

## 🗺️ Project Roadmap
This repository reflects the complete lifecycle of the forecasting system:
- **Phase 1: System Architecture & Planning (Completed)**
  - Defined forecasting horizons and designed the data pipeline flowchart.
- **Phase 2: Data Engineering (Completed)**
  - Sourced Kaggle solar plant telemetry and handled missing values.
  - Engineered cyclic time-based variables.
- **Phase 3: Ensemble Modeling (Completed)**
  - Developed, tuned, and compared Random Forest and XGBoost models.
- **Phase 4: Deep Learning & Comparative Analysis (Completed)**
  - Evaluated complex neural networks against tree-based ensembles (XGBoost selected for final deployment due to optimal balance of high accuracy and low latency).
- **Phase 5: Final Deployment & Exhibition (Completed)**
  - Deployed the `xgboost_solar_model.pkl` via a Gradio dashboard.

## 📊 Evaluation Metrics
The final XGBoost deployment model achieved the following metrics on unseen, chronologically split test data:
- **R-Squared (R²):** 0.9627 (Explains ~96% of the variance in power output)
- **Root Mean Squared Error (RMSE):** 1.59 kW (Ensures reliability during sudden weather shifts)
- **Mean Absolute Error (MAE):** 0.80 kW (Average magnitude of forecasting errors)

## 👥 Contributors
This project is developed as a Major Engineering Project for the B.Tech Computer Science and Engineering (Artificial Intelligence and Machine Learning) curriculum at IILM University.
- **Yasir Abbas Naqvi** – Roll No: 2410030883
- **Gopal Tomar** – Roll No: 2410030845
- **Kishan Tiwari** – Roll No: 2410030752

## 📂 Repository Structure
```text
├── data/                    # Dataset directory (Raw and Processed - excluded via .gitignore)
├── docs/                    # Architecture diagrams, design documents, and presentations
├── models/                  # Serialized models (e.g., xgboost_solar_model.pkl)
├── notebooks/               # Experimental Jupyter/Colab notebooks
│   ├── 01_EDA_and_Preprocessing.ipynb
│   ├── 02_Ensemble_Baselines_XGBoost_RF.ipynb
│   └── 03_Deep_Learning_Models.ipynb
├── src/                     # Modularized Python scripts for production
│   ├── data_loader.py       # Data ingestion and cleaning scripts
│   ├── feature_eng.py       # Feature selection and engineering
│   ├── model_trainer.py     # Training routines for ML and DL models
│   └── evaluate.py          # Metric calculations (R², RMSE, MAE)
├── app.py                   # Gradio web prototype deployment script
├── requirements.txt         # Project dependencies
└── README.md                # Project documentation
