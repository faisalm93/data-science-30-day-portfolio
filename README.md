# data-science-30-day-portfolio
30-day intensive data science portfolio with finance-focused, research-driven, and deployable projects.# Week 1 Case Study: Loan Default & Credit Risk Analysis

## 1. Problem Overview
Financial institutions must assess loan applications carefully to minimize default risk while maintaining fairness.
This project explores how data science can support loan approval decisions using historical applicant data.

---

## 2. Dataset Description
The dataset contains applicant-level financial and demographic information, including:
- Applicant and co-applicant income
- Loan amount and loan term
- Credit history
- Loan approval status

Target variables:
- Regression task: LoanAmount
- Classification task: Loan_Status (Approved / Not Approved)

---

## 3. Exploratory Data Analysis (EDA)
Key findings from EDA include:
- Credit history strongly correlates with loan approval
- Income alone does not determine approval
- Some low-income applicants are approved, suggesting multi-factor decision rules

EDA helped guide feature engineering and model selection.

---

## 4. Feature Engineering
Steps applied:
- Median imputation for numerical variables
- Mode imputation for categorical variables
- One-hot encoding for categorical features
- Feature scaling using StandardScaler

Assumptions:
- Missing values are missing at random
- Encoded categories sufficiently represent applicant profiles

---

## 5. Modeling Approach

### Regression
Models trained:
- Linear Regression
- Random Forest Regressor

Results:
- Random Forest captured nonlinear relationships better
- Linear Regression underfit complex financial patterns

### Classification
Models trained:
- Logistic Regression
- Random Forest Classifier

Evaluation metrics:
- Precision, Recall, F1-score
- Confusion Matrix
- ROC–AUC

Random Forest consistently outperformed Logistic Regression.

---

## 6. Model Explainability
SHAP was used to interpret model predictions.

Global insights:
- Credit history is the most influential feature
- Loan amount and income have context-dependent effects

Local explanations:
- Individual decisions can be explained transparently
- Improves trust and auditability of the model

---

## 7. Business & Research Implications
- The model aligns with real-world credit risk logic
- Explainability supports regulatory compliance
- Results demonstrate the feasibility of transparent AI in finance

---

## 8. Limitations
- Dataset size is limited
- Sensitive attributes (e.g., fairness metrics) not explicitly evaluated
- No hyperparameter tuning applied

---

## 9. Future Work
- Cost-sensitive classification
- Fairness and bias evaluation
- Deployment as a decision-support system
- Extension into longitudinal credit risk modeling

---

## 10. Conclusion
This project demonstrates a full, end-to-end finance data science workflow:
EDA → Feature Engineering → Modeling → Explainability → Interpretation.
It serves as a foundation for both industry applications and further academic research.

