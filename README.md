# Medical-Insurance-Claim-Fraud-Detection-Final-Project-
Medical Insurance Fraud Detection | Python, Pandas ,seaborn | 10,000 Rows, 16 Columns | EDA, outlier analysis,  Feature engineering &amp; Fraud risk scoring for insurance claim analysis

## 🎯 Objectives
1. To analyze medical insurance claims and identify fraud patterns
2. To clean data - handle missing values, duplicates, and outliers
3. To perform EDA to find relation between claim amount, incident type and fraud
4. To create new risk indicators like fraud_risk_score
5. To visualize fraud patterns with 10 charts and give recommendations to reduce loss

## 📊 Dataset Description
- **Source:** Kaggle - AI-based Medical Insurance Claim Fraud Detection
- **Size:** 10000 rows x 16 columns (Cleaned to 10,000 rows x 16 cols after feature engineering in this project)
- **Target Column:** `fraud_reported` - Y = Fraud, N = Genuine
- **Key Features:**
    - Money: total_claim_amount, injury_claim, property_claim
    - Customer: age, insured_sex, insured_education_level, insured_occupation
    - Incident: incident_type, incident_severity, incident_hour, authorities_contacted
    - Other: vehicle_age, policy_state, witnesses, collision_type

## 🔧 Methodology
1. **Data Cleaning:** Handled  missing values with mode & median, removed  duplicates, standardized categorical values, detected outliers using IQR method 
2. **Feature Engineering:** Created 4 new columns - claim_difference, age_group , is_high_claim, stay_category
3. **EDA:** Numerical Vs Numerical, Categorical vs Numerical, Categorical vs Categorical
4. **Visualization:** 10 charts - Histogram, KDE plot, Bar chart, count plot, scatter plot, correlation heatmap, interactive scatter plot chart using Matplotlib, Seaborn, Plotly

## 🔍 Key Findings
- Only 8% fraud but causes 30% financial loss
- Fraud average claim 85k vs Genuine 45k - almost double
- Night incidents: 22% fraud vs Morning 5%
- Total Loss severity: 28% fraud vs Minor Damage 4%
- No police report: 18% fraud vs Police contacted 6%
- fraud_risk_score >=3 captures 75% of all frauds
- Single vehicle collision is most faked (no witness)

## 📈 Visualizations
1. Histogram - claim_amt distribution

<img width="1280" height="473" alt="WhatsApp Image 2026-10-21 at 4 10 04 PM" src="https://github.com/user-attachments/assets/11923a6e-eeea-40a2-8774-26a87d744265" />


2.KDE Plot -



3.BOX Plot -




## 💡 Conclusion
Project successfully cleaned data, created 10 visualizations, identified total_claim_amount, incident_hour, incident_severity and authorities_contacted as key fraud factors. Model-ready dataset prepared with 0 missing values. This system helps insurance companies auto-flag high-risk claims and reduce losses.

**Future Scope:** Build Random Forest/XGBoost model to give 0-100 fraud probability, deploy Streamlit dashboard, real-time API integration.

## 🛠️ Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Colab Notebook



