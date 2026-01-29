# CMAPSS-LSTM-RUL-Prediction
# 🔧 Remaining Useful Life (RUL) Prediction on NASA CMAPSS Dataset

🚀 **Predictive Maintenance | Time-Series Deep Learning | LSTM**

## 📌 Overview
This repository presents a unified LSTM-based framework for predicting the Remaining Useful Life (RUL) of turbofan engines using the NASA CMAPSS dataset. All four subsets (FD001–FD004) are evaluated using a consistent and reproducible pipeline.

The project focuses on correct data parsing, RUL computation, sequence modeling, and NASA-standard engine-wise evaluation.

---

## 📊 Dataset
- **NASA CMAPSS** (FD001–FD004)
- Multivariate time-series sensor data
- Multiple operational and fault conditions

> ⚠️ Raw data is not included due to licensing restrictions.  
> Instructions for downloading the dataset are provided in the `data/` folder.

---

## 🧠 Methodology
- Correct CMAPSS parsing (`delim_whitespace=True`)
- RUL computation with **capping at 125 cycles**
- Feature normalization
- Sequence generation for LSTM
- Engine-wise test evaluation (NASA standard)

---

## 🏗 Model Architecture
- LSTM (100 units)
- Dropout (0.3)
- LSTM (50 units)
- Fully connected output layer

---

## ✅ Results Summary

| Dataset | Test MAE (cycles) |
|------|----------------|
| FD001 | ≈ **11** |
| FD002 | < 20 |
| FD003 | < 20 |
| FD004 | < 20 |

These results are comparable with strong baseline models reported in CMAPSS literature.

---

## 📁 Repository Structure
