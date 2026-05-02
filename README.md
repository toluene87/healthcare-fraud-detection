# 🏥 Healthcare Fraud Detection Analysis

## Project Overview

Healthcare fraud is a critical challenge that costs insurance systems billions annually. This project analyzes **10,000 healthcare claims** to identify patterns and key indicators of fraudulent billing activity using Microsoft Excel.

The goal was to explore the data, uncover fraud patterns across different dimensions, and surface actionable insights that could support fraud detection teams in prioritizing claims for investigation.

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data cleaning, pivot tables, charts, and dashboard

---

## 📁 Dataset

| Property | Detail |
|---|---|
| Total Records | 10,000 claims |
| Total Features | 20 columns |
| Fraud Rate | 8.29% (829 fraudulent claims) |
| Source | Synthetic healthcare claims dataset |

**Key columns include:**
- `Provider_ID`, `Claim_ID`, `Patient_Age`, `Patient_Gender`
- `Claim_Amount`, `Approved_Amount`, `Insurance_Type`
- `Provider_Specialty`, `Visit_Type`, `Diagnosis_Code`
- `Days_Between_Service_and_Claim`, `Number_of_Claims_Per_Provider_Monthly`
- `Chronic_Condition_Flag`, `Prior_Visits_12m`
- `Is_Fraud` — target variable (1 = Fraud, 0 = Legitimate)

---

## 🔍 Key Findings

### 1. Fraudulent Claims Cost Nearly Twice as Much
Fraudulent claims had an **average claim amount of $990.93**, compared to **$535.01** for legitimate claims — an **85% difference**. This suggests inflated billing as a primary fraud tactic.

### 2. General Practice Providers Had the Highest Fraud Rate
Among all specialties, **General Practice providers showed the highest fraud rate at 9.69%**, followed by Internal Medicine (8.67%) and Orthopedics (8.54%). Neurology had the lowest at 6.99%.

### 3. Medicare Claims Were Slightly More Fraud-Prone
**Medicare** had the highest fraud rate among insurance types at **8.45%**, with Medicaid close behind at 8.35%. Private insurance had the lowest at 8.23%.

### 4. Emergency Visit Claims Were Most Associated with Fraud
**Emergency visit claims** showed the highest fraud rate at **8.43%**, compared to Inpatient (8.23%) and Outpatient (8.21%) visits.

### 5. Claim Amount Range
Claim amounts ranged from **$60.21 to $6,590.70**, with a median of **$461.23**, indicating significant variability that warrants closer scrutiny on high-value outliers.

---

## 📊 Dashboard Highlights

The Excel dashboard includes:
- Fraud vs. Legitimate claim distribution (donut chart)
- Average claim amount by fraud status (bar chart)
- Fraud rate by Provider Specialty (bar chart)
- Fraud rate by Insurance Type (column chart)
- Fraud rate by Visit Type
- Slicers for dynamic filtering by Insurance Type and Visit Type

---

## 💡 Business Recommendations

1. **Flag high-value claims for review** — Claims significantly above the $990 average fraud amount should trigger automatic review
2. **Monitor General Practice providers closely** — They show the highest fraud rates and may benefit from enhanced auditing
3. **Prioritize Medicare claim audits** — Slight but consistent elevation in fraud rates warrants targeted oversight
4. **Investigate Emergency claims** — The higher fraud rate in emergency visits suggests potential abuse of emergency billing codes

---

## 📂 Project Structure

```
healthcare-fraud-detection/
│
├── healthcare_fraud_detection.csv   # Raw dataset
├── Healthcare_Fraud_Analysis.xlsx   # Excel workbook with analysis & dashboard
└── README.md                        # Project documentation
```

---
