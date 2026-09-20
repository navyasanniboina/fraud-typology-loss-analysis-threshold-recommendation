# 🏍️ Fraud Typology Loss Analysis & Threshold Recommendation
**End-to-End Data Analysis | Hypothesis Testing | Power BI Reporting**

---

## 📌 Project Overview
This project delivers an **end-to-end analytics solution** for identifying **fraud patterns** and modeling **claim severity** in the motor insurance domain.

It combines **statistical hypothesis testing in Python** with **multi-page Power BI dashboards** to transform raw claims data into **actionable, executive-ready insights** for fraud teams, underwriters, and business stakeholders.

The focus of this project is not just visualization, but **statistically validated decision-making**, closely aligned with real-world **insurance analytics workflows**.

---

## 🎯 Project Goals
- Evaluate whether **late claim reporting increases fraud risk**
- Analyze whether **older vehicles lead to higher claim severity**
- Identify **geographic fraud concentration** by city
- Assess whether **claim severity differs by accident type**
- Translate statistical results into **business-ready Power BI dashboards**
- Demonstrate **insurance-domain analytics thinking** suitable for fraud, risk, and underwriting roles

---

## ⭐ Key Highlights
- ✔ Conducted **4 statistical hypothesis tests** *(Z-test, T-test, Chi-square, ANOVA)*
- ✔ Built **5 structured Power BI report pages** for different stakeholders
- ✔ Added realistic **claim date** and **claim report date** logic for trend analysis
- ✔ Ensured **existing measures remained intact** while extending the data model
- ✔ Designed dashboards that show **validated insights, not raw statistics**
- ✔ Followed **enterprise BI best practices** *(separation of analysis & reporting)*

---

## 🧪 Hypotheses Tested

| # | Hypothesis | Statistical Test |
|---|-----------|------------------|
| 1 | Late reporting increases fraud | Two-Proportion Z-Test |
| 2 | Older vehicles have higher claim severity | Two-Sample T-Test |
| 3 | Fraud pattern differs by city | Chi-Square Test |
| 4 | Claim severity differs by accident type | One-Way ANOVA |

All hypotheses were tested at a **5% significance level**.  
Results with **p-value < 0.05** led to rejection of the null hypotheses.

---

## 🔍 Project Workflow & Steps

---

### 1️⃣ Data Understanding & Preparation
- Worked with motor insurance claims data containing:
  - Claim amount  
  - Vehicle age  
  - Reporting delay *(days_to_report)*  
  - City  
  - Accident type  
  - Garage type  
  - Fraud flag  
- Added:
  - `claim_date`
  - `claim_report_date`  
  using reporting-delay logic
- Ensured **original claim values were not altered**

---

### 2️⃣ Exploratory Data Analysis (Python)
- Analyzed distributions of:
  - Claim severity  
  - Reporting delay  
  - Vehicle age  
- Compared **fraud vs non-fraud** claims
- Identified early **behavioral and geographic risk indicators**

📓 **Notebook:** `motor_insurance.ipynb`

---

### 3️⃣ Hypothesis Testing (Python)
Performed statistical validation of business assumptions:

- **Z-Test:** Fraud rate comparison between late vs on-time claims  
- **T-Test:** Mean claim amount comparison for older vs newer vehicles  
- **Chi-Square:** Independence test between fraud occurrence and city  
- **ANOVA:** Severity comparison across accident types  

Results were interpreted using **p-values**, with clear **business conclusions documented**.

---

### 4️⃣ Power BI Data Modeling
- Loaded curated dataset into Power BI
- Created reusable **DAX measures** for:
  - Fraud Rate  
  - Claim Severity  
  - Risk Flags  
- Added a **date-aware model** using `claim_report_date`
- Safely changed data source **without impacting existing visuals or measures**

📊 **Power BI file:** `motor_insurance.pbix`

---

### 5️⃣ Power BI Report Design (5 Pages)

#### 📄 Page 1 — Executive Overview
<img width="1357" height="777" alt="image" src="https://github.com/user-attachments/assets/6284494c-9434-4760-887b-ebe80b5c7533" />

- Portfolio-level KPIs:
  - Total Claims  
  - Total Claim Amount  
  - Average Severity  
  - Fraud Rate  
  - Late Report Rate  
- Visual confirmation of **statistically validated insights**
- Designed for **30-second executive consumption**

---

#### 📄 Page 2 — Fraud Analysis Deep-Dive
<img width="1380" height="796" alt="image" src="https://github.com/user-attachments/assets/79639d0d-a49f-4d8b-a57a-8a534fd62293" />

- Fraud hotspots by city
- Late-reporting behavior analysis
- Scatter plots for behavioral investigation
- Supports **Z-test and Chi-square** results

---

#### 📄 Page 3 — Underwriting Risk Segmentation
<img width="1355" height="777" alt="image" src="https://github.com/user-attachments/assets/49fb7bf6-933a-498a-b167-c019b5ba9d3d" />

- High-risk claim percentage
- Risk matrices *(Vehicle Age × Accident Type)*
- City-level risk indices
- Converts analytics into **underwriting actions**

---

#### 📄 Page 4 — Ad-hoc Analyst Page
<img width="1346" height="790" alt="image" src="https://github.com/user-attachments/assets/f9acd0f9-1b5b-4f9f-a9a0-8ff90d901ac8" />

- Detailed claim-level table
- Flexible slicers and scatter plots
- Decomposition Tree for root-cause analysis
- Designed for exploration **without impacting executive views**

---

## 📊 Tools & Technologies
- **Python:** Pandas, NumPy, SciPy  
- **Statistical Methods:**
  - Z-Test  
  - T-Test  
  - Chi-Square  
  - ANOVA  
- **Power BI:**
  - DAX  
  - Multi-page dashboards  
  - Risk segmentation visuals  
- **Excel / CSV** for data integration

---

## 💼 Business Impact & Insights
- Late-reported claims show **significantly higher fraud probability**
- Vehicles older than **10 years** have higher average claim severity
- Fraud risk is **not evenly distributed across cities**
- Accident type is a **key driver of claim cost**
- Insights directly support:
  - Fraud investigation prioritization  
  - Underwriting rule refinement  
  - Risk-based pricing and reserving  

---

## 🧠 Key Learnings
- Importance of **statistical validation before visualization**
- Designing dashboards for **different stakeholder needs**
- Managing schema changes **without breaking Power BI measures**
- Translating analytics into **insurance business decisions**
- Applying hypothesis testing in a **real domain context**

---

## 📁 Project Artifacts
- 📓 **motor_insurance.ipynb** — EDA & Hypothesis Testing  
- 📊 **motor_insurance.pbix** — Power BI Report  

---

## 🚀 Next Steps
- Integrate **machine learning models** for fraud prediction
- Add **claim severity regression modeling**
- Implement **real-time fraud alerts** using streaming data
- Enhance underwriting views with **policy tenure and vehicle type**
- Extend analysis to include **loss ratios and reserve adequacy**

---

## 👤 Author
**Navya Sanniboina**  
Business Analyst | Power BI | SQL | Excel | Python | Statistics
