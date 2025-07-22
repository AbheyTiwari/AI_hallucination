# 🧠 AI Hallucination Risk Prediction — Notebook

This Jupyter Notebook presents the **backend model and analysis** for predicting AI hallucinations, using a mathematical framework that factors in:

- **Data Quality**
- **Model Confidence**
- **Input Ambiguity**
- **Adversarial Strength**

It complements the interactive [AI Hallucination Prediction Dashboard](./index.html), which visually demonstrates the same logic in real time.

---

## 📘 About This Notebook

The notebook includes:

- 📊 **Exploratory Data Analysis (EDA)** on synthetic or collected samples  
- 🧮 **Mathematical formulation** of hallucination risk  
- 🔍 **Feature engineering** (Z-score, interaction terms, normalization)  
- 📈 **Model training and evaluation** (e.g., logistic regression, GLMM)  
- 🎯 **Feature importance analysis** (using SHAP or coefficients)  
- ✅ **Performance metrics**: Accuracy, ROC-AUC, F1-Score  

---

## 🧪 Mathematical Model

We define the hallucination risk `H` as:

H = σ(αD + βM + γI + δA + ηC + θ(D·M) + φ(I·A) + ε)

Where:

- `σ` = Sigmoid function  
- `D` = Data Quality  
- `M` = Model Confidence  
- `I` = Input Ambiguity  
- `A` = Adversarial Strength  
- `ε` = Random noise / model bias  
- Interaction terms (`D·M`, `I·A`) capture non-linear dependencies

---

## 📂 Files in This Repository

| File | Description |
|------|-------------|
| `hallucination_model.ipynb` | 🧠 The core analysis and modeling notebook |
| `index.html` | 🎨 Interactive dashboard visualizing the same model |
| `README.md` | 📘 You're here |

---

## 📈 Model Summary

| Metric      | Value   |
|-------------|---------|
| Accuracy    | 94.2%   |
| ROC-AUC     | 0.91    |
| F1 Score    | 0.89    |
| Samples     | 200     |

---

## 🚀 How to Run

### Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `shap`

### Run with:

```bash
jupyter notebook AI_hallucination.ipynb
