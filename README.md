# 🏭 PHM Nexus: AI-Powered Predictive Asset Health & Warranty Intelligence Platform

## Overview

PHM Nexus is an AI-driven Predictive Health Management (PHM) platform designed to transform raw asset telemetry into actionable reliability, warranty, and financial intelligence.

The platform combines machine learning, deep learning, Digital Twin concepts, and fleet analytics to predict failures, estimate Remaining Useful Life (RUL), detect supplier quality issues, and optimize warranty decisions across connected assets such as EV batteries, industrial motors, turbines, and manufacturing equipment.

## Problem Statement

Most organizations still rely on reactive maintenance and fixed warranty policies. Failures are often identified only after breakdowns or warranty claims occur, leading to:

- High warranty costs
- Unplanned downtime
- Reduced asset reliability
- Inefficient maintenance planning
- Delayed detection of defective supplier batches

PHM Nexus addresses these challenges through predictive analytics and fleet-wide intelligence.

---

## Key Features

### 🔮 Predictive Failure Detection
Uses an XGBoost classifier to identify assets at risk of failure within a defined prediction window.

### ⏳ Remaining Useful Life (RUL) Estimation
Uses a Bidirectional LSTM neural network with attention mechanisms to estimate the remaining operational life of critical assets.

### 📊 Dynamic Warranty Intelligence
Generates real-time Warranty Risk Scores to support data-driven warranty and maintenance decisions.

### 🏭 Supplier Quality Intelligence
Detects abnormal failure patterns across supplier batches and estimates potential supplier chargeback liability.

### 🌐 Digital Twin Dashboard
Provides fleet-wide visualization of asset health, degradation trends, risk levels, and operational performance.

### ⚡ Real-Time Telemetry Simulation
Simulates IoT sensor streams to demonstrate live asset monitoring and predictive maintenance workflows.

---

## Solution Architecture

Data Sources → Feature Engineering → AI Models → Risk Intelligence Engine → Digital Twin Dashboard

### Pipeline

1. Telemetry data ingestion
2. Feature engineering and health indicator extraction
3. Failure classification using XGBoost
4. RUL prediction using Bidirectional LSTM
5. Warranty risk scoring
6. Supplier quality analytics
7. Fleet intelligence visualization

---

## Machine Learning Stack

### Model 1: Failure Classifier
- Algorithm: XGBoost
- Objective: Predict near-term asset failures
- Evaluation Metric: ROC-AUC

### Model 2: RUL Predictor
- Architecture: Bidirectional LSTM with Attention
- Objective: Remaining Useful Life estimation
- Evaluation Metric: Mean Absolute Error (MAE)

---

## Business Impact

PHM Nexus enables organizations to:

- Reduce warranty expenditure
- Minimize unplanned downtime
- Improve asset reliability
- Enable predictive maintenance
- Detect supplier quality issues earlier
- Improve lifecycle management decisions

### Demonstrated Results

| Metric | Result |
|----------|----------|
| Failure Prediction AUC | 94.6% |
| RUL Prediction MAE | 6.74 Cycles |
| Estimated Fleet Reserve Savings | $70,646 |
| Potential Supplier Chargebacks | $2,088,571 |
| Downtime Reduction Potential | ~40% |

---

## Technology Stack

### Programming Language
- Python

### Machine Learning
- XGBoost
- Scikit-learn

### Deep Learning
- PyTorch

### Data Processing
- NumPy
- Pandas

### Visualization
- Matplotlib
- Seaborn
- Plotly

### Dashboard & Interaction
- IPyWidgets

---

## Project Structure

```text
PHM_Nexus/
├── notebooks/
│   └── tata-innovent_hackathon.ipynb
├── models/
│   ├── xgb_failure_classifier.pkl
│   ├── lstm_best.pt
│   └── feature_scaler.pkl
├── reports/
│   ├── supplier_quality_report.csv
│   ├── fleet_risk_matrix.csv
│   └── simulation_telemetry.json
├── data/
│   └── phm_nexus_full_dataset.csv
└── README.md
```

## Future Enhancements

- Edge AI deployment using TensorFlow Lite / ONNX
- Federated Learning across distributed fleets
- Real-time cloud integration
- Physics-informed Digital Twins
- Enterprise warranty management integration

## Use Cases

- Electric Vehicles
- Commercial Fleets
- Aerospace Systems
- Wind Turbines
- Industrial Equipment
- Smart Manufacturing

## Authors

Developed as part of the Tata Technologies InnoVent Hackathon initiative.
