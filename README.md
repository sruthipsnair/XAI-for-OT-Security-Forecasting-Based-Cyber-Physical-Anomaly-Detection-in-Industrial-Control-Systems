# XAI-for-OT-Security-Forecasting-Based-Cyber-Physical-Anomaly-Detection-in-Industrial-Control-Systems
Vertical distributed architecture using Edge TCNs and Cloud GDN with XAI integrated for anomaly detection on the SWaT dataset.



## Overview
This repository contains a Distributed Spatio-Temporal architecture designed for anomaly detection in Industrial Control Systems (ICS). The framework moves away from centralized processing and horizontal federated learning (like FedeX) to optimize Operational Technology (OT) network constraints. 

## Architecture Design
- **Edge Predictor (TCN):** Lightweight Temporal Convolutional Networks deployed directly on Programmable Logic Controllers (PLCs) forecast physical states. This vertical isolation reduces the network transmission payload to just 4 bytes per second per node, eliminating network congestion on fragile OT LANs.
- **Cloud Aggregator (GDN):** A Graph Deviation Network located in the central Security Operations Center (SOC) maps the macro-level physical topology, catching multi-stage cyberattacks without the mathematical aggregation bias found in traditional Federated Averaging.
- **Intrinsic Spatio-Temporal XAI:** An integrated forensic engine that bypasses static tools like SHAP. It mathematically backtracks to identify the exact stealth window onset, isolates the physical root cause, and condenses over 40,000 raw anomalous seconds into 274 actionable forensic operator reports.

## Performance Metrics
- **Accuracy:** 98.35%
- **F1-Score:** 0.78
- **Alert Fatigue Reduction:** Utilizes a dynamic 9.5-sigma threshold to suppress ambient plant noise, resulting in extremely low False Positives (9,836 out of 1.4 million normal operational seconds).

## Dataset
This model is trained and evaluated on the **Secure Water Treatment (SWaT)** dataset provided by the iTrust Centre for Research in Cyber Security at the Singapore University of Technology and Design (SUTD). The dataset is a high-fidelity replica of a modern six-stage water treatment facility.
- **Dataset Access:** https://www.kaggle.com/datasets/vishala28/swat-dataset-secure-water-treatment-system

## Repository Structure
- `model_implementation.ipynb`: Complete Kaggle notebook containing the Edge TCN extractors, Cloud GDN aggregator, and Intrinsic XAI backtracking logic.
