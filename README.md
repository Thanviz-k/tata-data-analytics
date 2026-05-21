# Geldium Credit Risk — Tata Data Analytics Programme

An end-to-end data analytics project simulating a real-world credit delinquency use case for **Geldium Financial Services**, completed as part of the Tata Data Analytics Virtual Experience Programme.

---

## Project Overview

| Task | Deliverable | Description |
|------|-------------|-------------|
| Task 1 | EDA | Exploratory data analysis of customer financial & behavioural dataset |
| Task 2 | `Task2_ModelPlan_Completed.docx` | Predictive modelling plan using XGBoost for delinquency forecasting |
| Task 3 | `Task3_BusinessSummaryReport.docx` | Stakeholder-ready business summary report for Head of Collections |
| Task 4 | `Task4_AI_Collections_Strategy.pptx` | Executive briefing deck for an AI-powered autonomous collections system |

---

## Key Findings

- **Top risk factors:** Missed payments (12-month count), credit utilisation >70%, and debt-to-income ratio >50%
- **Recommended model:** XGBoost — balances accuracy, native missing-value handling, and SHAP explainability for regulatory compliance
- **SMART recommendation:** Proactively contact customers when credit utilisation crosses 70%, targeting a 15% reduction in 90-day delinquency within 6 months

---

## AI Collections System Design (Task 4)

The proposed system operates in four stages:

1. **Data Ingestion** — credit score, utilisation, missed payments, 6-month payment history
2. **Risk Scoring** — XGBoost outputs a delinquency probability (0–1) per customer, updated monthly
3. **Automated Action** — score ≥0.65 → agent call; 0.45–0.65 → SMS/email nudge; <0.45 → no action
4. **Learning Loop** — outcomes feed back into monthly model retraining

### Responsible AI Guardrails
- Disparate impact checks across customer sub-groups (trigger threshold: ratio < 0.80)
- SHAP-based plain-language explanations for every prediction
- Risk Committee sign-off required before each model version goes live
- Annual independent ethics audit

---

## Tools & Concepts Used

`XGBoost` `SHAP` `SMOTE` `AUC-ROC` `F1 Score` `Fairness Auditing` `SMART Framework` `Responsible AI` `Microsoft Word` `PowerPoint`

---

*This project was completed as part of the Tata Group Data Analytics Virtual Experience Programme.*
