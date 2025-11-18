# Toward Trustworthy Clinical Decision Support: Robust and Explainable Machine Learning for Stroke Risk Stratification

![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Scikit--learn%20%7C%20Pandas%20%7C%20SHAP-orange.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository contains the complete code and research materials for developing a robust and explainable machine learning framework for stroke risk prediction. This project addresses critical challenges in clinical AI, including severe class imbalance and the need for model transparency, with the goal of creating a trustworthy tool for clinical decision support.

## 📝 Project Goal

The primary objective is to build a model that not only predicts stroke risk with high accuracy but is also **reliable** and **interpretable**. We aim to move beyond simple accuracy metrics to focus on performance measures that matter in a clinical setting (like Recall) and provide clear, patient-specific explanations for the model's predictions.

## 🔬 Key Contributions

1.  **Systematic Imbalance Handling:** A comprehensive comparative analysis of techniques like SMOTE, ADASYN, and cost-sensitive learning to establish an evidence-based strategy for imbalanced clinical datasets.
2.  **Clinically Actionable Interpretability:** Implementation of a SHAP (SHapley Additive exPlanations) module to provide both global feature importance insights and local, patient-specific risk factor analysis.
3.  **Robust Preprocessing Pipeline:** A reproducible data preprocessing pipeline using MICE imputation and feature scaling to enhance model performance and generalizability.

## 🚀 Getting Started

### Prerequisites

This project was developed in a Google Colab environment. All required libraries are listed in the notebook and can be installed via pip.
- Python 3.8+
- pandas
- scikit-learn
- imbalanced-learn
- shap
- matplotlib & seaborn

### Running the Code

1.  Clone this repository.
2.  Download the **Stroke Prediction Dataset** from [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset) and place `healthcare-dataset-stroke-data.csv` in the root directory.
3.  Open and run the `antorResearchML.ipynb` Jupyter Notebook in an environment like Google Colab, JupyterLab, or VS Code. The notebook is structured to run sequentially from top to bottom.

## 📊 Results

Our experiments show that a **Logistic Regression** model trained on **SMOTE-balanced data** achieves the highest recall for stroke detection. The SHAP analysis on our Random Forest model successfully identified clinically relevant risk factors, demonstrating the framework's ability to produce transparent and trustworthy results.

---
_Feel free to add a "Contact" or "Citation" section if you have a pre-print or publication link later on._
