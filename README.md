![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Domain](https://img.shields.io/badge/Domain-Predictive%20Maintenance-purple)

# 🔧 Remaining Useful Life (RUL) Prediction on NASA CMAPSS

### 🚀 Predictive Maintenance | Time-Series Deep Learning | LSTM

## 🎯 Why This Project Matters

Predicting Remaining Useful Life (RUL) is a core task in predictive maintenance — helping industries anticipate failures, minimize downtime, and reduce costs. This repository provides a comprehensive and reproducible benchmark across all CMAPSS subsets (FD001–FD004) using LSTM, adhering to NASA-standard evaluation practices.

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

## ✅ Results Summary

| Dataset | Difficulty Level | Test MAE (cycles) |
|---------|------------------|-------------------|
| **FD001** | Easy | **≈ 11** |
| **FD002** | Medium | < 20 |
| **FD003** | Medium | < 20 |
| **FD004** | Hard | < 20 |

> All results follow NASA-standard engine-wise evaluation.
These results are comparable with strong baseline models reported in CMAPSS literature.

---

## 📁 Repository Structure
