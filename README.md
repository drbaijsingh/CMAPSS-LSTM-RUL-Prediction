![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Topic](https://img.shields.io/badge/Domain-Predictive%20Maintenance-purple)

# 🔧 Remaining Useful Life (RUL) Prediction on NASA CMAPSS

### 🚀 Predictive Maintenance | Time-Series Deep Learning | LSTM

## 🎯 Why This Project Matters

Predicting the Remaining Useful Life (RUL) of complex systems like aircraft engines is a core task in predictive maintenance. Accurate RUL prediction helps reduce unplanned downtime, optimize maintenance schedules, and cut costs in industrial assets.

This repository provides:
- A reproducible LSTM pipeline for all NASA CMAPSS subsets (FD001–FD004)
- NASA-standard engine-wise performance evaluation
- Strong results across multiple operating and fault conditions


## 📌 Overview
This repository presents a unified LSTM-based framework for predicting the Remaining Useful Life (RUL) of turbofan engines using the NASA CMAPSS dataset. All four subsets (FD001–FD004) are evaluated using a consistent and reproducible pipeline.

The project focuses on correct data parsing, RUL computation, sequence modeling, and NASA-standard engine-wise evaluation.

## 📊 Dataset
- **NASA CMAPSS** (FD001–FD004)
- Multivariate time-series sensor data
- Multiple operational and fault conditions


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

| Dataset | Difficulty | Test MAE (± cycles) |
|---------|------------|---------------------|
| **FD001** | Easy | ≈ **11** |
| **FD002** | Medium | < 20 |
| **FD003** | Medium | < 20 |
| **FD004** | Hard | < 20 |

> Results use NASA standard evaluation (engine-wise).


---

## 📁 Repository Structure
notebooks/ → Jupyter notebooks for each CMAPSS subset (FD001–FD004)
results/ → Saved plots and metric summaries
data/ → Instructions for downloading NASA CMAPSS data (no raw data included)
requirements.txt → Python dependencies

## ▶️ How to Run

✅ 5) Add “How to Run” Block

Right after the structure:

## ▶️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/drbaijsingh/CMAPSS-LSTM-RUL-Prediction.git


Install dependencies:

pip install -r requirements.txt


Download CMAPSS data as documented in data/README.md

Open the appropriate notebook and run


This improves usability dramatically.

---

## ✅ 6) Add License (Recommended)

At the bottom add a license badge (you already have one) but also include a simple MIT license text.

Create a file named **LICENSE** in your repo with:

```text
MIT License
