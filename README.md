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

<img width="813" height="586" alt="WhatsApp Image 2026-10-21 at 4 10 01 PM" src="https://github.com/user-attachments/assets/5c46ef41-3a34-45d5-91b8-bd31dbdd8595" />





2.KDE Plot -Age distribution



<img width="822" height="586" alt="WhatsApp Image 2026-10-21 at 4 10 01 PM (1)" src="https://github.com/user-attachments/assets/941a7dda-c191-471f-9e49-e8dba4b83602" />




3.BOX Plot - claim_amt



<img width="847" height="520" alt="WhatsApp Image 2026-10-21 at 4 10 02 PM" src="https://github.com/user-attachments/assets/706777fc-b27d-430d-8199-0469f683bc9b" />




4.COUNT PLOT - stay category




<img width="819" height="580" alt="WhatsApp Image 2026-10-21 at 4 10 02 PM (2)" src="https://github.com/user-attachments/assets/6f036714-0da1-465b-a436-054329ccba57" />




5.CORRELATION HEATMAP 



<img width="927" height="711" alt="WhatsApp Image 2026-10-21 at 4 10 03 PM (1)" src="https://github.com/user-attachments/assets/3454ce09-fc61-475a-a41e-72e713f901cc" />




6. SCATTER PLOT

   

   <img width="931" height="586" alt="WhatsApp Image 2026-10-21 at 4 10 03 PM" src="https://github.com/user-attachments/assets/36c91126-79fe-4091-a7ab-10bc2a255221" />


   

7. BAR CHART - hospital type analysis

   

   <img width="1280" height="473" alt="WhatsApp Image 2026-10-21 at 4 10 04 PM" src="https://github.com/user-attachments/assets/72055130-cb43-4c03-8c47-3e0626ac7f44" />

   
   
8. INTERACTIVE SCATTER CHART-Fraud detection

    
   
   -<img width="1280" height="474" alt="WhatsApp Image 2026-10-21 at 4 10 03 PM (3)" src="https://github.com/user-attachments/assets/23f8fa9a-05fc-47b7-a77a-e5d6d8351e33" />

   

   9.CATEGORICAL VS NUMERICAL BOX PLOT

   

   <img width="769" height="468" alt="WhatsApp Image 2026-10-21 at 4 10 03 PM (2)" src="https://github.com/user-attachments/assets/3c68011a-36e4-4093-925e-be7818d2edb4" />


   

10.BAR CHART




<img width="862" height="558" alt="WhatsApp Image 2026-10-21 at 4 10 02 PM (1)" src="https://github.com/user-attachments/assets/f414e45e-f224-4a5e-8ffc-8b5bf63aa991" />





## 💡 Conclusion
Project successfully cleaned data, created 10 visualizations, identified total_claim_amount, incident_hour, incident_severity and authorities_contacted as key fraud factors. Model-ready dataset prepared with 0 missing values. This system helps insurance companies auto-flag high-risk claims and reduce losses.

**Future Scope:** Build Random Forest/XGBoost model to give 0-100 fraud probability, deploy Streamlit dashboard, real-time API integration.

## 🛠️ Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Colab Notebook



