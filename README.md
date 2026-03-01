# Large-Scale Survival Modeling for Reliability Prediction

## Overview

This project explores advanced survival modeling techniques for reliability prediction across:

- Physics-based semiconductor degradation simulation
- NASA CMAPSS turbofan degradation datasets (FD001–FD004)
- Static Cox Proportional Hazards models
- DeepSurv (Neural Cox model)
- LSTM-based temporal survival modeling
- Large-scale training on 130k+ time-series sequences

The work demonstrates that temporal survival modeling significantly outperforms static survival approaches for degradation forecasting.

---
## Research Abstract

This project investigates large-scale survival modeling for reliability prediction using both physics-based simulation and real-world aerospace degradation data (NASA CMAPSS).

We first demonstrate that static survival models (Cox Proportional Hazards and DeepSurv) fail to capture degradation dynamics in time-series settings (C-index ≈ 0.47–0.52). We then develop a temporal LSTM-based survival framework trained on 130,000+ sequences across multiple operating conditions (FD001–FD004), achieving a concordance index of 0.85.

We further explore Transformer-based survival modeling and introduce physics-guided monotonicity regularization to enforce degradation consistency. Experimental results highlight the importance of temporal inductive bias in modeling monotonic failure processes.

This work bridges statistical survival analysis, deep learning, and reliability engineering for predictive maintenance applications.

## Key Results

| Model | Dataset | Concordance Index |
|--------|----------|------------------|
| Cox (Static) | CMAPSS | 0.47 |
| DeepSurv (Static) | CMAPSS | 0.52 |
| LSTM Survival | FD001 | 0.81 |
| LSTM Survival (Big Data) | FD001–FD004 | 0.85 |

---

## Technical Contributions

- Demonstrated failure of static survival modeling on time-series degradation data
- Built physics-informed synthetic reliability simulator
- Implemented neural survival modeling using PyTorch
- Scaled temporal survival modeling to 130k+ sequences
- Mini-batch training with Cox partial likelihood loss
- Multi-dataset generalization across operating conditions

---

## Technologies Used

- Python
- PyTorch
- Lifelines (Survival Analysis)
- NumPy / Pandas
- Scikit-Learn
- Time-Series Modeling
- LSTM Neural Networks

---

## Future Work

- Transformer-based survival modeling
- Attention-based degradation learning
- Graph-temporal survival models
- Cross-domain reliability modeling

---

## 📊 Key Results

| Model | Dataset | Test Concordance (C-Index) |
|-------|---------|----------------------------|
| Cox Proportional Hazards | CMAPSS (FD001) | 0.46 |
| DeepSurv | CMAPSS (FD001) | 0.51 |
| LSTM Survival | CMAPSS (FD001) | 0.81 |
| Large-Scale LSTM Survival | CMAPSS (FD001–FD004) | **0.85** |

Temporal survival modeling significantly outperforms static survival models for degradation forecasting.


## 🔬 Methodology

1. Physics-informed degradation simulation
2. Static survival modeling (Cox PH)
3. Neural Cox model (DeepSurv)
4. Temporal sequence modeling (LSTM Survival)
5. Large-scale training on 130k+ sequences

The framework demonstrates the importance of time-dependent modeling in predictive maintenance systems.



## Author

Satwik Pvnr  
B.Tech ECE  
Research focus: Reliability modeling, survival analysis, temporal deep learning
