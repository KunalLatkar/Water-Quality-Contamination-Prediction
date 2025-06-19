#  Water Quality Contamination Prediction – ML Models

This repository contains machine learning models built to predict whether a water sample is **contaminated or safe**, using environmental monitoring data collected across India (2012–2023). The dataset used for training and evaluation was obtained from a separate open-source repository (see below).

---

##  Dataset Source

The full dataset, preprocessing steps, and feature documentation are hosted here:  
🔗 **[Water Quality Dataset (India) – Gathering & Preprocessing](https://github.com/KunalLatkar/RiverWaterQualityDataset)**

This includes:
- Min/Max values of physical and chemical water properties (pH, DO, BOD, etc.)
- Station metadata (state, location, year)
- A derived binary target column: `Contaminated` (1 = unsafe, 0 = safe)

---

##  Objective

To train, evaluate, and compare different classical machine learning algorithms for:
- **Binary classification** of water contamination
- **Feature importance analysis**
- **Model evaluation using accuracy, precision, recall, F1-score, and confusion matrix**

---

##  Models Implemented

| Model Name               | Description                                              |
|--------------------------|----------------------------------------------------------|
| Logistic Regression       | Baseline interpretable model                             |
| Decision Tree Classifier  | Simple tree-based model for rule inference               |
| Random Forest             | Ensemble of decision trees, robust to overfitting        |
| AdaBoost Classifier       | Boosted ensemble with weighted error correction          |
| XGBoost Classifier        | Highly optimized gradient boosting algorithm             |

All models were trained on the same dataset split and evaluated using consistent metrics.

---

##  Features Used

- Temperature (Min/Max)
- Dissolved Oxygen (Min/Max)
- pH (Min/Max)
- Conductivity (Min/Max)
- BOD (Min/Max)
- Nitrate (Min/Max)
- Coliform and Streptococci counts (Min/Max)
- Year, State (as encoded categorical features)

