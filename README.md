# 📊 HR Analytics & Employee Attrition Risk Modeling (ML & Multi-Dimensional Visualization)

An end-to-end Exploratory Data Analysis (EDA) and Machine Learning interpretability suite analyzing employee turnover, career stagnation, salary compression, work-life balance, and satisfaction metrics using Python, Seaborn, Plotly, and Scikit-Learn in Google Colab.

---

## 📌 Project Overview

Employee turnover creates substantial organizational costs and operational disruption. This project delivers a comprehensive HR analytics suite to evaluate workforce attrition drivers, identify high-risk employee cohorts, isolate compensation/promotion bottlenecks, and build interpretable retention classification rules.

---

## 🎯 Objective

* Parse multi-attribute workforce records safely with automated encoding handlers
* Quantify the impact of overtime, commute distance, salary slabs, and job roles on turnover rates
* Train Random Forest and Decision Tree models to score feature importances and establish explicit retention rules
* Build polar radar profiles, interactive parallel categories, and 3D risk feature spaces to map employee retention profiles
* Analyze career stagnation trends through promotion decay curves and empirical cumulative probability distributions (ECDF)

---

## 📊 Dataset Schema

* **Key Attributes:**
  * **Demographics & Travel:** `Age`, `AgeGroup`, `Gender`, `MaritalStatus`, `DistanceFromHome`, `BusinessTravel`
  * **Job & Department:** `Department`, `JobRole`, `JobLevel`, `SalarySlab`, `EducationField`
  * **Compensation & Performance:** `MonthlyIncome`, `DailyRate`, `HourlyRate`, `PercentSalaryHike`, `PerformanceRating`, `StockOptionLevel`
  * **Satisfaction & Engagement:** `EnvironmentSatisfaction`, `JobSatisfaction`, `RelationshipSatisfaction`, `WorkLifeBalance`, `JobInvolvement`
  * **Tenure & Career Progression:** `TotalWorkingYears`, `YearsAtCompany`, `YearsInCurrentRole`, `YearsSinceLastPromotion`, `YearsWithCurrManager`, `NumCompaniesWorked`
  * **Target Variable:** `Attrition` (`Yes` / `No` ➔ Encoded to `1` / `0`)

---

## 📈 Complete Analytical & Machine Learning Suite (13 Cells)

1. **Ingestion & Target Encoding:** Dataset loader & `Attrition_Numeric` feature engineering
2. **Organizational Breakdown:** Departmental turnover rate (%) & salary slab distribution
3. **Compensation & Workload Impact:** Monthly income boxplots & overtime attrition rates
4. **Role Satisfaction Matrix:** Job role attrition vs. multi-metric satisfaction heatmaps
5. **Predictive Drivers:** Random Forest feature importance ranking
6. **Cohort Behavioral Profiles:** Polar radar chart comparing retained vs. attrited employees
7. **Organizational Career Flow:** Interactive Plotly parallel categories diagram (`Department` ➔ `Role` ➔ `Salary Slab` ➔ `Attrition`)
8. **Tenure Decay Distributions:** Faceted KDE curves across promotion rates and manager tenure
9. **Bi-Directional Risk Profile:** Directional correlation analysis (Turnover Risk Factors vs. Retention Protective Factors)
10. **Interactive 3D Risk Space:** Plotly 3D scatter plot (`MonthlyIncome` vs. `TotalWorkingYears` vs. `DistanceFromHome`)
11. **Income Compression Analysis:** Boxen plots tracking monthly income spread across job levels
12. **Rule Interpretability:** Visual Decision Tree retention flowchart (Depth = 3)
13. **Cumulative Probabilities:** ECDF probability curves for total working years and income levels

---

## 🛠 Tech Stack

* **Language:** Python
* **Environment:** Google Colab
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Random Forest, Decision Tree, Metrics)
* **Visualization:** Matplotlib, Seaborn, Plotly Express

---

## 🤖 Key Insights

* **Compensation & Overtime Pressure:** Employees working overtime combined with lower monthly income tiers show the highest attrition density.
* **Career Stagnation:** Retention risk increases sharply among employees who have gone 4+ years without a promotion or role shift.
* **Managerial Dynamics:** Extended tenure with the same manager without internal progression creates burnout drift, particularly in junior job levels.
* **Protective Factors:** Higher stock option levels, elevated work-life balance ratings, and closer proximity to home serve as primary retention anchors.

---

## 📊 Results

* Identified top predictive turnover drivers using Random Forest feature rankings
* Extracted actionable, human-readable HR retention rules using visual Decision Trees
* Mapped interactive 3D risk spaces and career flow pipelines for non-technical stakeholders

---

## 🔮 Future Improvements

* Build an interactive Streamlit dashboard for real-time HR turnover risk scoring
* Implement SHAP (SHapley Additive exPlanations) values for granular employee-level turnover predictions
* Deploy survival analysis models (Cox Proportional Hazards) to predict employee tenure life expectancy
