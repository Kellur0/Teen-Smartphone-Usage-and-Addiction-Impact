# Teen-Smartphone-Usage-and-Addiction-Impact
Analyzed Kaggle’s Teen Phone Addiction dataset (3,000 teens, 42 features) to explore links between smartphone habits, academic performance, and mental health. Applied clustering, correlation, and regression in Python to uncover usage patterns and provide actionable insights for healthier tech habits.



# Teen Phone Addiction Analysis

Analyzed Kaggle’s **Teen Phone Addiction** dataset to explore how smartphone habits relate to **academic performance** and **mental health** among teens. This repo includes data preprocessing, clustering, correlation analysis, and regression models built in Python (Google Colab).

---

## 📌 Overview
- **Dataset size:** 3,000 teens (ages 12–18)
- **Original features:** 25 → **42 after preprocessing** (dummy variables added)
- **Focus:** Links between phone use patterns, grades, anxiety, depression, self‑esteem
- **Key insight:** Outcomes depend more on **purpose & patterns** (e.g., social media vs. education) than total screen time.

---

## 📊 Dataset
- Source: Kaggle — Teen Phone Addiction
- URL: https://www.kaggle.com/datasets/sumedh1507/teen-phone-addiction
- Notable fields (subset):
  - `Daily_Usage_Hours`, `Weekend_Usage_Hours`, `Screen_Time_Before_Bed`
  - `Time_on_Social_Media`, `Time_on_Gaming`, `Time_on_Education`
  - `Phone_Checks_Per_Day`, `Apps_Used_Daily`, `Addiction_Level`
  - Outcomes: `Academic_Performance`, `Anxiety_Level`, `Depression_Level`, `Self_Esteem`
- Privacy: Dropped `Name` and `Location` columns.

---

## 🧪 Methodology
1. **Preprocessing**
   - Cleaned CSV, handled types; converted categorical variables to **dummy variables**.
   - Verified **0 missing values**.
2. **Clustering (K‑means)**
   - Elbow method to choose `k` (found 3–4 useful).
   - Identified profiles: *Gaming‑focused*, *Social‑media‑focused*, *Education‑focused*, *Mixed*.
3. **Correlation & Statistical Tests**
   - Pearson correlations across usage features & addiction.
   - One‑Way **ANOVA**, **Kruskal‑Wallis**, and **Dunn‑Bonferroni** (post‑hoc) for academic differences by addiction level.
4. **Regression Models**
   - Multiple regression for **Academic Performance** and **Mental Health Risk** (composite).
   - Grade‑level interaction effects (7th–12th).

---

## ✅ Results (Highlights)
- **Academic performance** shows **minimal** direct relationship to total screen time.
- **Addiction Level** strongly predicts **mental‑health risk**, especially in grades **7, 9, and 10**.
- **Social‑media‑heavy** patterns: lower grades, higher depression, lower self‑esteem.
- **Gaming** can be a healthy outlet (higher academics, lower anxiety/depression in some clusters).
- **Educational use** boosts academics but may increase **anxiety** (pressure/overload).

---
