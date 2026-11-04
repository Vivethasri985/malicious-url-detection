# 🔐 An Explainable ML & DL Framework for Malicious URL Detection

> Presented at **ICMLDE 2025** | Published in : [Procedia Computer Science, 2026 - Elsevier](https://www.sciencedirect.com/science/article/pii/S1877050926018685)
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)
![XGBoost](https://img.shields.io/badge/XGBoost-Best%20Model-green?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-98.44%25-brightgreen?style=flat-square)
![Status](https://img.shields.io/badge/Status-Research%20%7C%20Pre--Publication-orange?style=flat-square)

---

## 📌 Overview

Cyberattacks are at an all-time high, with global losses expected to exceed **$10.5 trillion by 2025**. Over **900 million phishing attempts** were recorded in 2024 alone — and **80% of malicious links are zero-day threats** that traditional methods fail to catch.

This project presents a **hybrid ML/DL framework** that detects malicious URLs with high accuracy while remaining **transparent and explainable** using SHAP and LIME — addressing the critical black-box problem in existing approaches.

---

## 👥 Authors

| Name | Role |
|------|------|
| Amitha Mahesh | Co-author |
| Nitheka A | Co-author |
| S Shivvanii | Co-author |
| Vivethasri C | Co-author |
| S Manimaran | Co-author |

---

## 🧠 Methodology

### Dataset
- Combination of **Manu Siddhartha's Kaggle dataset** and **Hannousse et al.**
- Preprocessing: tokenization, normalization, outlier removal

### Feature Selection
- **RFECV** (Recursive Feature Elimination with Cross-Validation)
- Optimal subset selected from **4000+ features**

### Models Trained
| Model | Type |
|-------|------|
| Random Forest | Machine Learning |
| XGBoost | Machine Learning |
| Artificial Neural Network (ANN) | Deep Learning |
| Convolutional Neural Network (CNN) | Deep Learning |

### Explainability
- **LIME** — Local surrogate model explaining individual URL predictions
- **SHAP** — Global feature importance showing what drives model decisions

### Deployment
- Real-time URL detection pipeline with **192ms latency**

---

## 📊 Results

### Performance Metrics

| Model | Accuracy | F1 Score | Precision | Recall |
|-------|----------|----------|-----------|--------|
| **XGBoost** | **0.9844** | **0.9734** | 0.9619 | **0.9852** |
| CNN | 0.9839 | 0.9725 | 0.9637 | 0.9814 |
| ANN | 0.9832 | 0.9711 | **0.9672** | 0.9750 |
| Random Forest | 0.9785 | 0.9636 | 0.9443 | 0.9836 |

> ✅ **XGBoost** achieved the best overall performance — outperforming the baseline (Hani et al., 95.49% accuracy) across all metrics.

### Explainability Highlight (LIME)
Top features driving XGBoost predictions:
- `path_length` — strongest indicator of malicious URLs
- `url_length` — second most influential feature
- Token patterns like `://`, `.co`, `htt` also contribute significantly

---

## 🔍 Key Contributions

- ✅ Adaptive feature selection using RFECV (vs. static feature sets in prior work)
- ✅ Hybrid ML + DL comparison on the same dataset
- ✅ Full explainability via SHAP (global) + LIME (local)
- ✅ Real-time detection validated at **192ms latency**
- ✅ Outperforms baseline across all four metrics

---

## 📚 Citation

> Paper presented at **ICMLDE 2025**. Full citation will be updated upon publication.

---

## ⚠️ Note

This repository currently contains the README and results. Full source code will be made available upon paper publication.

---

## 🏷️ Tags

`Machine Learning` `Deep Learning` `Explainable AI` `Cybersecurity` `XGBoost` `SHAP` `LIME` `URL Detection` `Phishing` `RFECV` `Python` `ICMLDE2025`
