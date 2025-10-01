# Advanced Data Mining Models for Customer Behavior Analytics

## Abstract 📄
This project explores **advanced data mining models** applied to information systems and customer behavior analytics.  
We implement and compare multiple approaches, including **Churn Classification (XGBoost + SHAP)**, **Survival Analysis (Kaplan–Meier, CoxPH)**, **Uplift Modeling**, and **Sequential Recommendation Models (GRU4Rec, BERT4Rec)**.  
The analysis leverages datasets such as **Telco Churn**, **Criteo Uplift**, and **RetailRocket**, and demonstrates how advanced predictive modeling can improve customer retention and engagement.

**Keywords**: Data Mining, XGBoost, SHAP, Kaplan–Meier, CoxPH, Uplift Modeling, GRU4Rec, BERT4Rec, Customer Analytics

---

## Table of Contents 📋
* [Introduction](#introduction)
* [Datasets](#datasets)
* [Models Implemented](#models-implemented)
* [Results & Insights](#results--insights)
* [Conclusion & Future Work](#conclusion--future-work)
* [References](#references)

---

## Introduction 💡
Modern businesses face challenges in understanding **customer churn, retention, and behavior**.  
This project applies advanced modeling approaches to:  
- Predict churn and key customer risks.  
- Estimate survival probabilities.  
- Evaluate the impact of marketing interventions.  
- Provide sequential product recommendations.  

---

## Datasets 📂
We used publicly available datasets from Kaggle for analysis:  

- **[Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)** – Customer churn data with demographics, contract info, and billing details.  
- **[Criteo Uplift Modeling](https://www.kaggle.com/datasets/gauravduttakiit/criteo-uplift-modeling)** – Dataset for uplift modeling and treatment effect estimation.  
- **[RetailRocket Recommender System Dataset](https://www.kaggle.com/datasets/retailrocket/ecommerce-dataset)** – Real-world e-commerce session and interaction logs for sequential recommendation tasks.  

---

## Models Implemented ⚙️
### A. Churn Classification  
- **Model**: XGBoost + SHAP interpretability  
- **Goal**: Predict churn risk and explain features driving it  

### B. Survival Analysis  
- **Models**: Kaplan–Meier & Cox Proportional Hazards  
- **Goal**: Estimate customer survival probability over time  

### C. Uplift Modeling  
- **Models**: S-Learner, T-Learner, X-Learner, Causal Forest  
- **Goal**: Measure the **incremental effect** of marketing interventions  

### D. Sequential Modeling  
- **Models**: GRU4Rec / BERT4Rec  
- **Goal**: Provide personalized product recommendations  

---

## Results & Insights 📊
- XGBoost + SHAP achieved **ROC-AUC ≈ 0.815** for churn prediction.  
- CoxPH survival analysis highlighted key risk factors:  
  - **Senior Citizen** → ~1.6x higher churn risk.  
  - **Monthly Charges** significantly affect survival.  
- Uplift modeling produced **Uplift@30% ≈ 0.036**, demonstrating measurable impact of marketing interventions.  
- GRU/BERT-based models achieved strong **MRR@5 ≈ 0.729** in sequential recommendations.  

---

## Conclusion & Future Work 🏁
- Advanced models provide actionable insights into **churn, retention, and marketing strategy**.  
- Combining survival, uplift, and recommendation models enables **holistic customer lifecycle management**.  
- Future Work:  
  - Apply on larger, real-world enterprise datasets.  
  - Extend uplift modeling with deep learning approaches.  
  - Integrate sequential models into production recommender systems.  

---

## 📓 Projects & Files

### 1. Advanced Data Mining Models (Notebook)
[Jupyter Notebook](Advanced_Data_Mining_Models.ipynb)  

Run Online 🚀  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<YOUR_USERNAME>/<YOUR_REPO>/blob/main/Advanced_Data_Mining_Models.ipynb)  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<YOUR_USERNAME>/<YOUR_REPO>/HEAD?labpath=Advanced_Data_Mining_Models.ipynb)

---

## References 📚
- Verbeke et al. (2012) *Customer churn prediction models with advanced rule induction techniques*  
- Lundberg & Lee (2017) *SHAP: Unified approach to interpreting model predictions*  
- Lee et al. (2018) *DeepHit: Deep learning survival analysis*  
- Künzel et al. (2019) *Meta-learners for heterogeneous treatment effects*  
- Hidasi et al. (2016) *GRU4Rec*  
- Sun et al. (2019) *BERT4Rec*
