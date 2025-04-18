
# 🦷 Prediction Tool for Non-Carious Cervical Lesions (NCCLs)

This project leverages machine learning to predict **volume loss in experimental tooth specimens**, helping identify conditions that have higher potential for non-carious cervical lesions (NCCLs) development. By simulating lesion progression and analyzing influencing variables, the tool aims to **optimize in vitro testing** and significantly reduce experimental costs and time.

To our knowledge, there are no prior studies in literature that use predictive modeling for estimating NCCL progression based on controlled abrasivity factors. This makes the project an early step toward integrating data science into preventive dental research.
---

## Project Objective

To develop a predictive model that estimates volume loss under various experimental conditions using structured data from past studies. The model assists in prioritizing  scenarios for testing, with the goal of improving efficiency in dental research.

---

## Data Overview

- **Source**: In vitro experimental dataset based on past abrasivity studies
- **Variables include**:
  - Toothpaste type
  - Bristle stiffness
  - Brushing force
  - Slurry concentration
  - Number of brushing strokes
- **Target**: Volume loss in mm³ (indicative of tooth wear)
---

## 🛠 Methods Used

- Data Cleaning and Feature Engineering
- Exploratory Data Analysis (EDA)
- Model Training:
  - Random Forest Regressor
  - Gradient Boosting Regressor
  - XG Boost
- Model Evaluation using:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
  - R² Score
- Feature Importance Ranking

---

## 📈 Results & Insights

- Best model achieved R² ≈ 0.70, demonstrating good predictive power
- Toothpaste type and number of strokes were among the top contributing features
- Feature importance visualization helped interpret model predictions and optimize experiment design

---

## 💡 Key Takeaways

- This predictive tool can reduce experimental test load and helps researchers focus on high-risk combinations early on to avoid tedious lab experiments
- Contributes to cost-efficient and data-driven abrasivity research, which could lead to the development of a Clinical decision support tool to track these insidious lesions.

---

## 📦 Tools & Technologies

- Python (pandas, scikit-learn, matplotlib, seaborn)
- Jupyter Notebook
- Random Forest, Gradient Boosting, SVR

---
## ⚠️ Limitations

- The dataset used is small, which may limit the generalizability of the model
- The data lacks **clinical factors** such as patient-specific oral hygiene behavior, enamel thickness, or occlusal load
- This version is intended for **preclinical research purposes** and not for clinical deployment

