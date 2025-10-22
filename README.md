# 🌌 Advanced Photometric Analysis for Predicting Specific Star Formation Rates in Large Galaxies

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)]()
[![Framework](https://img.shields.io/badge/Framework-Scikit--Learn%20%7C%20TensorFlow%20%7C%20PyTorch-orange)]()
[![Dataset](https://img.shields.io/badge/Dataset-SDSS--DR7-lightgrey)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)]()

---

## 📌 Overview
This study predicts **Specific Star Formation Rates (sSFRs)** from **photometric data** in **SDSS‑DR7** using a combination of **machine learning (ML)** and **deep learning (DL)** models.  
The workflow is implemented in two phases:

- **Phase I** → Baseline modelling on the original dataset.
- **Phase II** → Synthetic data augmentation using a **Gaussian Copula** model to improve generalisation.

---

## ✨ Key Findings
- **SVR** achieved the best performance on the original dataset:  
  - MAE = 0.2413  
  - MSE = 0.1167  
  - RMSE = 0.3416  
  - R² = 0.1895
- **Random Forest** achieved the best generalisation after synthetic data augmentation:  
  - MAE = 0.3094
- **DBSCAN clustering** identified high‑variability sSFR regions, guiding future astronomical observations.
- An **interactive visualisation tool** was developed for exploring predictions and spatial trends.


---

## 🛰 Data Source
- **Photometric data from over 27 million galaxies** in **SDSS‑DR7**  
- Subset used: 1,048,576 galaxies with features including RAdeg, DEdeg, photoz, quality flag, and sSFR

---

## ⚙️ Models Implemented
- **Support Vector Regression (SVR)**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Decision Tree Regressor**
- **Linear Regression**
- **Lasso & Ridge Regression**
- **Long Short‑Term Memory (LSTM) Networks**
- **Classical Deep Learning Models**

## Flow Chart of Phase I

  <img width="565" height="649" alt="image" src="https://github.com/user-attachments/assets/ee1e187e-cd7b-463d-896d-a6097c41b952" />


---

## 📊 Performance Summary

| Phase | Model          | MAE     | MSE     | RMSE    | R²      | Notes |
|-------|---------------|---------|---------|---------|---------|-------|
| I     | SVR           | **0.2413** | 0.1167  | 0.3416  | 0.1895  | Best on original data |
| II    | Random Forest | 0.3094  | 0.1889  | 0.4346  | 0.0415  | Best with synthetic data |

---

## 🔍 Clustering & Visualisation
- **DBSCAN** used to detect high‑variability sSFR regions (e.g., Clusters 34, 11, 6)
- Interactive tool features:
  - Filter by RA/DE
  - Zoom & pan
  - Highlight DBSCAN clusters
  - Overlay photometric redshift distributions
 
<img width="847" height="612" alt="image" src="https://github.com/user-attachments/assets/b5fb976b-63cd-48fb-a95a-2003afb17182" />

---

## 🗺️ Regions of Interest (ROI) Summary
| Cluster ID | RA Range (deg) | Dec Range (deg) | Notable Characteristics |
|------------|---------------|-----------------|-------------------------|
| 34         | 150–160       |  2–10           | High sSFR variance, potential merger candidates |
| 11         | 210–220       | –5–5            | Dense galaxy grouping, elevated starburst activity |
| 6          |  45–55        | –10–0           | Outliers in colour–magnitude space, possible AGN contamination |

> These ROIs can be prioritised for **follow‑up spectroscopic surveys** to validate ML/DL‑based predictions.

## Flow Chart showing Phase II

<img width="580" height="661" alt="image" src="https://github.com/user-attachments/assets/f8d8430b-a4e2-467c-8de3-b7736a70d93b" />

---

## 🤝 Contributing
Contributions are welcome!  
- Fork the repository  
- Create a feature branch  
- Submit a pull request  
- Or open an issue for suggestions and improvements

---

## 📬 Contact
**Prasanth Ayitapu**  
📧 [karthikeya23p@gmail.com](mailto:[karthikeya23p@gmail.com)

---

## 💡 Skills Demonstrated
- Large‑scale astronomical data preprocessing
- Regression modelling (ML & DL)
- Synthetic data generation (Gaussian Copula)
- Clustering analysis (DBSCAN)
- Interactive scientific visualisation
- Translating model outputs into actionable observational targets
