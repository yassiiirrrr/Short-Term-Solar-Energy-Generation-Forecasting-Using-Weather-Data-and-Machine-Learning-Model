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

## 🗺️ Project Roadmap
This repository reflects the complete lifecycle of the forecasting system, structured into the following phases:

* **Phase 1: System Architecture & Planning (Completed)**
  * Defining forecasting horizons and selecting target features.
  * Designing the data flow and model pipeline architecture.
* **Phase 2: Data Engineering (Completed)**
  * Sourcing Kaggle solar plant telemetry and weather datasets.
  * Handling missing values, normalizing features, and engineering time-based variables.
* **Phase 3: Baseline Modeling (Completed)**
  * Developing and tuning Random Forest and XGBoost regression models.
  * Benchmarking initial predictions against validation sets.
* **Phase 4: Advanced Deep Learning (In Progress)**
  * Designing and training artificial neural networks using TensorFlow and Keras.
  * Comparing deep learning performance against ensemble baselines.
* **Phase 5: Final Evaluation & Delivery (Upcoming)**
  * Compiling final metrics.
  * Finalizing project documentation and preparing the system for demonstration.

## 📊 Evaluation Metrics
The models are evaluated against the test dataset using the following regression metrics to ensure predictive accuracy:
* **R-Squared (R²):** Measures the proportion of variance in power output predictable from the weather data.
* **Root Mean Squared Error (RMSE):** Penalizes larger forecasting errors to ensure model reliability during sudden weather shifts.
* **Mean Absolute Error (MAE):** Represents the average magnitude of forecasting errors.


## 👥 Contributors
This project is developed as a Major Engineering Project for the B.Tech Computer Science and Engineering (Artificial Intelligence and Machine Learning) curriculum.

* **[Yasir Abbas Naqvi]** – Roll No: [2410030883]
* **[Gopal Tomar]** – Roll No: [2410030845]
* **[Kishan Tiwari]** – Roll No: [2410030752]

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

