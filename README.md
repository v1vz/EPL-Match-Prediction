# Predicting Football Match Outcomes with Explainable Machine Learning

This repository reproduces the experiments from  
**“Predicting Football Match Outcomes with Explainable Machine Learning:  
A Data- & Knowledge-Driven Framework, Risk-Aware Staking, and League-Scale Evaluation.”**

---

## 🔍 Overview
- **Goal:** Predict Win/Draw/Loss (W/D/W) for Premier League 2020/21 fixtures.  
- **Approach:** Knowledge-driven feature engineering + calibrated tree models.  
- **Core models:** Logistic Regression, Random Forest, CatBoost, XGBoost.  
- **Evaluation:** Accuracy, Macro-F1, Log-Loss, Brier Score, Ranked Probability Score.  
- **Explainability:** SHAP/permutation importances for global + local interpretation.  
- **Risk-aware staking:** Kelly-based position sizing on calibrated probabilities.

---

## 🗂️ Repository structure
| Folder | Purpose |
|---------|----------|
| `data/` | (Optional) sample structure & schema — actual data scraped from FBref. |
| `notebooks/` | Jupyter notebooks for feature engineering, training, and explainability. |
| `src/` | Modular Python scripts for preprocessing, modeling, and staking. |
| `configs/` | YAML configuration of seeds, splits, and hyperparameters. |
| `outputs/` | Saved metrics, figures, and logs. |

---

## ⚙️ Installation
```bash
git clone https://github.com/YOURUSERNAME/epl-match-outcome-ml.git
cd epl-match-outcome-ml
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
