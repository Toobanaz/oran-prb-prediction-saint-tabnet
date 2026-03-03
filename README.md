# Intelligent PRB Demand Prediction using SAINT and TabNet

This repository implements transformer-based and tabular deep learning models 
for predicting requested radio resources in O-RAN network slicing environments.

## 📌 Problem Statement

In Open Radio Access Networks (O-RAN), efficient allocation of Physical Resource 
Blocks (PRBs) is critical for network slicing and 6G resource optimization. 
Over-provisioning leads to inefficiency, while under-provisioning impacts QoS.

This project predicts requested resources using tabular learning models.

## 🧠 Models Implemented

- SAINT (Self-Attention and Intersample Transformer)
- TabNet
- Baseline comparisons

## 📊 Dataset

The dataset (`slices.csv`) contains tabular slice-level features including:

- Slice ID
- QoS indicators
- Traffic demand features
- Historical resource usage
- Target: Requested PRBs

## 📈 Evaluation Metrics

- MSE
- R² Score
- MAPE

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:
   pip install -r requirements.txt
3. Run the notebook:
   Github Predicting requested resources - SAINT and TabNet.ipynb

## 🔬 Research Context

This work is part of ongoing research on intelligent resource prediction 
for O-RAN slicing using transformer-based tabular models.
