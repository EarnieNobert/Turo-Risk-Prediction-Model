# Turo Risk Prediction Model

This project is a machine learning-based booking risk decision engine inspired by vehicle-sharing marketplace platforms like Turo.

It is designed to evaluate booking risk at checkout by predicting:

- the probability of a claim
- the expected cost if a claim occurs
- the expected financial loss of the booking

The system then uses these outputs to generate a decision such as:

- APPROVE  
- APPROVE_WITH_CONDITIONS  
- REVIEW  
- DECLINE  

---

## Demo Video

Watch the full demo here:  
(*****)

---

## Overview

In real-world marketplace platforms, claim data is private and not publicly available.

To address this, I built a synthetic dataset that simulates realistic booking scenarios, including:

- driver history  
- trip behavior  
- vehicle class  
- market location  
- claim outcomes  
- claim costs  

This allows the system to model both risk probability and financial impact.

---

## Key Features

- Synthetic data generation for marketplace bookings  
- XGBoost model for claim probability prediction  
- Probability calibration for improved reliability  
- XGBoost model for claim severity (cost prediction)  
- Expected loss calculation (probability × cost)  
- Policy engine for booking decisions  
- SHAP explainability for model transparency  

---

## Workflow

1. Generate synthetic booking and claims data  
2. Preprocess numerical and categorical features  
3. Train claim probability model  
4. Calibrate predicted probabilities  
5. Train severity model on claim costs  
6. Calculate expected loss  
7. Apply decision logic using policy engine  
8. Explain predictions using SHAP  

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- SHAP  
- Jupyter Notebook  

---

## Why This Project Matters

This project demonstrates how machine learning can be applied to real-world risk assessment problems by combining:

- predictive modeling  
- financial reasoning  
- business decision logic  
- model explainability  

into a single system. also how creative modifictions can further enhance the overall effectiveness and undertandability of models.

---

## Future Improvements

- Deploy as an API for real-time risk scoring  
- Add dashboard for operational monitoring  
- Introduce A/B testing for policy thresholds  
- Implement model monitoring and drift detection  
