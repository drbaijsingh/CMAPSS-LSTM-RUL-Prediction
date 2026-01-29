![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Domain](https://img.shields.io/badge/Domain-Predictive%20Maintenance-purple)

# 🔧 Remaining Useful Life (RUL) Prediction on NASA CMAPSS

### 🚀 Predictive Maintenance | Time-Series Deep Learning | LSTM

## 🎯 Why This Project Matters
Predicting the Remaining Useful Life (RUL) of complex systems such as aircraft engines is a core task in predictive maintenance. Accurate RUL prediction helps reduce unplanned downtime, optimize maintenance schedules, and lower operational costs in industrial assets.

This repository provides:
- A reproducible LSTM-based pipeline for all NASA CMAPSS subsets (FD001–FD004)
- NASA-standard engine-wise performance evaluation
- Strong results across multiple operating and fault conditions

---

## 📌 Overview
This repository presents a unified LSTM-based framework for predicting the Remaining Useful Life (RUL) of turbofan engines using the NASA CMAPSS dataset. All four subsets (FD001–FD004) are evaluated using a consistent and reproducible pipeline.

The project emphasizes correct data parsing, RUL computation, sequence modeling, and NASA-standard engine-wise evaluation.

---

## 📊 Dataset
- **NASA CMAPSS** (FD001–FD004)
- Multivariate time-series sensor data
- Multiple operational and fault conditions

> ⚠️ Raw dataset files are not included due to NASA licensing.

---

## 🧠 Methodology
- Correct CMAPSS parsing using `delim_whitespace=True`
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

| Dataset | Difficulty | Test MAE (cycles) |
|--------|-----------|------------------|
| **FD001** | Easy | **≈ 11** |
| **FD002** | Medium | < 20 |
| **FD003** | Medium | < 20 |
| **FD004** | Hard | < 20 |

> Results follow NASA-standard engine-wise evaluation.

---

## 📁 Repository Structure
