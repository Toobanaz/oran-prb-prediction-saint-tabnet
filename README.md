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

## 📊 Dataset Source

The dataset used in this study is derived from the ColO-RAN framework:

M. Polese, L. Bonati, S. D’Oro, S. Basagni, and T. Melodia,
“ColO-RAN: Developing machine learning-based xApps for open RAN closed-loop control on programmable experimental platforms,”
IEEE Transactions on Mobile Computing, 2022.

The ColO-RAN dataset was collected using the Colosseum wireless network emulator and represents a multi-cell 5G scenario with:

- 7 Base Stations (BS1–BS7)
- 42 User Equipments (UEs)
- Multiple traffic classes: eMBB, URLLC, and mMTC

## 📁 Data Processing for This Study

For this implementation, we use a combined dataset constructed from
78,561 slice-level telemetry records extracted from 41 CSV log files
located in:

shed0/tr0/exp1/

These logs contain:

- Traffic statistics
- RAN performance metrics
- Slice-level resource utilization
- QoS indicators over time

The data has been preprocessed and transformed into a structured
tabular format (`slices.csv`) suitable for supervised learning and
PRB demand prediction using transformer-based tabular models.

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
