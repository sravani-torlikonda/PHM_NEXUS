# 🏭 PHM Nexus: AI-Powered Predictive Asset Health & Warranty Intelligence Platform

## Overview

PHM Nexus is an advanced Predictive Health Management (PHM) platform that transforms raw asset telemetry into actionable reliability, maintenance, warranty, and financial intelligence.

The platform combines Machine Learning, Deep Learning, Digital Twin concepts, and Fleet Analytics to predict failures, estimate Remaining Useful Life (RUL), identify supplier quality issues, and optimize warranty decisions across connected assets such as electric vehicles, industrial equipment, turbines, manufacturing systems, and critical infrastructure.

By shifting organizations from reactive maintenance to predictive asset intelligence, PHM Nexus enables smarter lifecycle management, improved reliability, and reduced operational costs.

---

## Problem Statement

Most organizations still rely on reactive maintenance strategies and fixed warranty policies. Critical component failures are often identified only after breakdowns or warranty claims occur, leading to:

* High warranty expenditure
* Unplanned downtime
* Reduced asset reliability
* Inefficient maintenance scheduling
* Increased operational costs
* Delayed identification of defective supplier batches

Modern connected assets generate vast amounts of operational data, but much of this data remains underutilized for proactive decision-making.

PHM Nexus addresses these challenges through AI-driven predictive analytics and fleet-wide asset intelligence.

---

## Key Features

### 🔮 Predictive Failure Detection

Utilizes an XGBoost-based machine learning model to identify assets at elevated risk of failure before breakdowns occur.

### ⏳ Remaining Useful Life (RUL) Estimation

Employs a Bidirectional LSTM neural network with attention mechanisms to estimate the remaining operational life of critical components.

### 📊 Dynamic Warranty Intelligence

Generates real-time Warranty Risk Scores that support data-driven warranty planning and maintenance decisions.

### 🏭 Supplier Quality Intelligence

Identifies abnormal failure patterns across supplier batches and estimates potential financial impact associated with defective components.

### 🌐 Digital Twin Dashboard

Provides fleet-wide visualization of asset health, degradation trends, operational performance, and risk distribution.

### ⚡ Real-Time Telemetry Simulation

Simulates IoT sensor streams to demonstrate live monitoring, anomaly detection, and predictive maintenance workflows.

### 📈 Fleet Risk Analytics

Enables asset segmentation based on health, risk levels, utilization patterns, and predicted failure probability.

---

## Solution Architecture

```text
Telemetry Sources
        │
        ▼
Data Ingestion & Processing
        │
        ▼
Feature Engineering
        │
 ┌──────┴──────┐
 ▼             ▼
Failure      RUL
Prediction   Prediction
(XGBoost)    (Bi-LSTM)
 └──────┬──────┘
        ▼
Risk Intelligence Engine
        │
 ┌──────┼─────────┐
 ▼      ▼         ▼
Warranty  Supplier  Fleet
Scoring   Analytics Intelligence
        │
        ▼
Digital Twin Dashboard
```

---

## Machine Learning Stack

### Failure Prediction Model

* Algorithm: XGBoost Classifier
* Objective: Predict near-term asset failures
* Evaluation Metric: ROC-AUC

### Remaining Useful Life Model

* Architecture: Bidirectional LSTM with Attention
* Objective: Estimate Remaining Useful Life (RUL)
* Evaluation Metric: Mean Absolute Error (MAE)

### Risk Intelligence Engine

* Warranty Risk Scoring
* Fleet Segmentation
* Supplier Quality Assessment
* Financial Impact Analysis

---

## Business Impact

PHM Nexus enables organizations to:

* Reduce warranty expenditure
* Minimize unplanned downtime
* Improve asset reliability
* Enable predictive maintenance strategies
* Detect supplier quality issues earlier
* Optimize maintenance scheduling
* Improve lifecycle management decisions
* Enhance operational efficiency

### Demonstrated Results

| Metric                                 | Result      |
| -------------------------------------- | ----------- |
| Failure Prediction AUC                 | 94.6%       |
| RUL Prediction MAE                     | 6.74 Cycles |
| Estimated Fleet Reserve Savings        | $70,646     |
| Potential Supplier Liability Detection | $2,088,571  |
| Downtime Reduction Potential           | ~40%        |

---


## Project Structure

```text
PHM_Nexus/
├── notebooks/
│   └── phm_nexus_analysis.ipynb
│
├── models/
│   ├── xgb_failure_classifier.pkl
│   ├── lstm_best.pt
│   └── feature_scaler.pkl
│
├── reports/
│   ├── supplier_quality_report.csv
│   ├── fleet_risk_matrix.csv
│   └── simulation_telemetry.json
│
├── data/
│   └── phm_nexus_full_dataset.csv
│
├── requirements.txt
└── README.md
```

---

## Future Enhancements

* Edge AI deployment using ONNX Runtime and TensorRT
* Federated Learning for distributed fleet intelligence
* Physics-Informed Digital Twin integration
* Real-time cloud deployment
* Streaming analytics using Apache Kafka
* Enterprise Asset Management (EAM) integration
* Automated maintenance recommendation engine

---

## Potential Applications

* Electric Vehicles (EVs)
* Commercial Vehicle Fleets
* Aerospace Systems
* Wind Turbines
* Industrial Motors
* Manufacturing Equipment
* Smart Factories
* Energy Infrastructure

---


## Contributors

* **Sravani** – Machine Learning, Data Engineering, Analytics, System Integration
 
  GitHub: https://github.com/sravani-torlikonda
  
* **Rishik** –  Deep Learning, Warranty Intelligence, Dashboard Development, Documentation
  GitHub: https://github.com/rishii-25

## Disclaimer

The results, financial estimates, and performance metrics presented in this project are based on the dataset, simulation environment, and evaluation methodology used within this implementation. Actual outcomes may vary depending on deployment conditions and operational environments.

---

## License

This project is intended for educational, research, and demonstration purposes.
