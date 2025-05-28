
# UK Board-Level Social Mobility Prediction: A Machine Learning Study

*Author: Khalid · Date: 2025-05-28*

---

## 🧠 Project Overview

This project explores social mobility in the UK by modelling the likelihood of individuals reaching **board-level roles** at major organisations, based on educational background, region, gender, and sector. Inspired by the **Sutton Trust’s Elitist Britain (2019)** report, we simulate this analysis using extended synthetic data to demonstrate how machine learning can quantify elite access patterns.

---

## 📊 Data Source & Simulation

- **Real Report Base**: Sutton Trust (2019), *Elitist Britain*.
- **Synthetic Extension**: Simulated board-level outcomes (`IsBoardMember`) based on trends observed in the original report.
- **Key Features**: School type, university type, sector, gender, region.

All synthetic data is clearly marked and generated only for skill demonstration purposes.

---

## 🔍 Exploratory Analysis

- Board-level roles disproportionately correlate with:
  - **Private school education**
  - **Attendance at Oxbridge**
  - **Certain sectors (Media, Law, Politics)**
- Regional imbalance also evident.

---

## ⚙️ Model Training & Evaluation

### Model 1: Baseline (No Class Balancing)

- **Accuracy**: 70.5%
- **Precision (Board Success)**: 37.3%
- **Recall (Board Success)**: 8.4% (very low)
- **F1 Score**: 13.7%

### Model 2: Improved (Class Weights Applied)

- **Accuracy**: 57.8%
- **Precision (Board Success)**: 33.9%
- **Recall (Board Success)**: **54.1%**
- **F1 Score**: **41.7%** ✅

Significant improvement in identifying true success cases. Demonstrates model fairness awareness.

---

## 📌 Explainability

### Feature Importance (via Random Forest)
1. Sector
2. Region
3. School Type
4. University Type
5. Gender

### PDP Plots
[✓] Show how each of the top 3 features affect board-level prediction scores.

---

## 🧠 Insights

- Education and region continue to define access to top roles.
- Predictive models show we can simulate risk scores for elite outcomes.
- With real data access, this could become a board diversity audit tool.

---

## 🛠️ What’s Next?

- Add real HR data where possible
- Build a shareable dashboard or API
- Use for DEI (Diversity, Equity, Inclusion) consulting

---

## 📂 Repo Contents

- `Simulated_Elitist_Britain_Dataset.csv`
- `UK_Board_Social_Mobility_ML_Study.ipynb`
- `PDP_Top_Features.png`
- `README.md`

---

## 🔗 Contact

Built by Khalid — Independent ML Consultant & Data Strategist  
LinkedIn / GitHub: *Insert handles here*

---

