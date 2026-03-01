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

## Author

Satwik Pvnr  
B.Tech ECE  
Research focus: Reliability modeling, survival analysis, temporal deep learning
