# 🏦 Credit Risk Modelling

A comprehensive credit risk modelling framework using machine learning techniques to estimate **Probability of Default (PD)**, **Loss Given Default (LGD)**, and **Exposure at Default (EAD)**. The project also includes scorecard generation and **Population Stability Index (PSI)** analysis for model stability over time.

---

## 📁 Repository Contents

- credit_risk_dataset.csv     # Raw loan-level data
- code.ipynb     # Initial EDA and preprocessing
- pd.ipynb     # PD model development
- pd_scorecard.ipynb     # Scorecard generation from PD
- lgd_ead_el.ipynb     # LGD, EAD & Expected Loss models
- psi_check.ipynb     # PSI for model stability monitoring

---

## 🚀 Project Goals

- Build predictive models for key credit risk parameters:
  - Probability of Default (PD)
  - Loss Given Default (LGD)
  - Exposure at Default (EAD)
- Create a transparent scorecard based on PD estimates
- Evaluate model performance and stability over time

---

## 🔍 Methodology

### 1. Data Preprocessing
- Missing value imputation
- Categorical encoding
- Outlier treatment
- Feature scaling & selection

### 2. Model Development
- **PD**: Logistic Regression / Tree-based classifiers
- **LGD**: Beta Regression / Random Forest Regressor
- **EAD**: Linear Regression
- Scorecard: Binning + Weight of Evidence (WoE)

### 3. Model Evaluation
- **Classification**: AUC, Gini Index, Confusion Matrix
- **Regression**: R², MSE
- **Stability**: PSI (Population Stability Index)

---

## 📊 Results Summary

| Metric        | PD Model | LGD Model | EAD Model |
|---------------|----------|-----------|-----------|
| AUC Score     | 0.78     | -         | -         |
| Accuracy      | ~85%     | -         | -         |
| R² Score      | -        | 0.65      | 0.70      |
| PSI           | Stable   | -         | -         |

---

## 📈 Sample Scorecard Bands

| Credit Score | Risk Level |
|--------------|------------|
| 750 - 850    | Low Risk   |
| 650 - 749    | Moderate   |
| 550 - 649    | High Risk  |
| Below 550    | Very High  |

---

## 🛠️ Technologies Used

- **Language**: Python
- **Libraries**: pandas, numpy, scikit-learn, matplotlib, seaborn
- **Environment**: Jupyter Notebook

