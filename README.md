# Small Business Administration (SBA) Loan Analysis

## Overview

This project analyzes **U.S. Small Business Administration (SBA) loan data (1987–2014)** to uncover patterns in loan approvals, disbursements, and repayment outcomes.

The analysis integrates **data cleaning, exploratory data analysis (EDA), feature importance evaluation, and machine learning models** to generate actionable insights.

### Key Results

* **XGBoost** achieved the best classification performance:

  * ROC-AUC: 0.977
  * Accuracy: 94%
* **Gradient Boosting** produced the lowest RMSE for predicting loan approval amounts
* Key factors influencing repayment include:

  * Loan term
  * Bank affiliation
  * Industry type
  * Approved loan amount

This project demonstrates how **predictive analytics can support better lending decisions and reduce default risk**.

---

## Background

Small businesses play a significant role in:

* Economic growth
* Job creation
* Local development

Many rely on SBA-backed loans for startup capital, expansion, or recovery from financial challenges. The SBA guarantees a portion of these loans, reducing lender risk; however, defaults still result in financial losses.

### Loan Outcomes

* **PIF (Paid in Full):** Loan successfully repaid
* **CHGOFF (Charged Off):** Loan defaulted

Analyzing historical data helps identify risk patterns, borrower behavior, and predictive indicators of default.

---

## Research Problem

Despite the availability of large historical datasets, many lending decisions still rely on manual evaluation or broad rule-based systems. This approach often overlooks subtle but important patterns in the data.

This project addresses the following:

1. Identification of factors influencing loan repayment
2. Prediction of loan outcomes (PIF vs CHGOFF)
3. Modeling of key financial variables such as approval amounts
4. Development of data-driven decision support for lending

---

## Objectives

* Conduct exploratory analysis of SBA loan data
* Identify factors affecting loan repayment outcomes
* Develop classification models to predict loan status (PIF vs CHGOFF)
* Develop regression models to predict SBA-approved loan amounts

---

## Data Description

* **Source:** [https://pengdsci.github.io/datasets](https://pengdsci.github.io/datasets)
* **Period:** January 1987 – December 2014
* **Observations:** 899,164
* **Variables:** 27 (categorical and numerical)
* **Target Variable:** `MIS_Status`

The dataset includes borrower details, loan characteristics, bank information, and repayment outcomes.

### Notes

* The dataset contains historical formatting inconsistencies
* Only SBA-guaranteed loans are included

---

## Variable Summary

| Variable          | Type     | Description                      |
| ----------------- | -------- | -------------------------------- |
| LoanNr_ChkDgt     | Text     | Unique Loan Identifier           |
| Name              | Text     | Borrower Name                    |
| City              | Text     | Borrower City                    |
| State             | Text     | Borrower State                   |
| Zip               | Text     | Zip Code                         |
| Bank              | Text     | Lending Bank                     |
| BankState         | Text     | Bank Location                    |
| NAICS             | Text     | Industry Classification Code     |
| ApprovalDate      | Date     | Loan Approval Date               |
| ApprovalFY        | Text     | Fiscal Year                      |
| Term              | Numeric  | Loan Term (months)               |
| NoEmp             | Numeric  | Number of Employees              |
| NewExist          | Text     | 1 = Existing, 2 = New            |
| CreateJob         | Numeric  | Jobs Created                     |
| RetainedJob       | Numeric  | Jobs Retained                    |
| FranchiseCode     | Text     | Franchise Indicator              |
| UrbanRural        | Text     | 1 = Urban, 2 = Rural             |
| RevLineCr         | Text     | Revolving Credit Indicator (Y/N) |
| LowDoc            | Text     | LowDoc Program Indicator (Y/N)   |
| ChgOffDate        | Date     | Charge-Off Date                  |
| DisbursementDate  | Date     | Disbursement Date                |
| DisbursementGross | Currency | Amount Disbursed                 |
| BalanceGross      | Currency | Outstanding Balance              |
| MIS_Status        | Text     | Loan Status (Target Variable)    |
| ChgOffPrinGr      | Currency | Charged-Off Amount               |
| GrAppv            | Currency | Approved Loan Amount             |
| SBA_Appv          | Currency | SBA Guaranteed Amount            |

---

## Project Highlights

### Data Cleaning

* Handling missing values
* Standardizing inconsistent formats
* Cleaning categorical variables

### Exploratory Data Analysis

* Trends by year, industry, and geography
* Distribution of loan outcomes
* Identification of default patterns

### Predictive Modeling

* Classification: PIF vs CHGOFF
* Regression: Loan approval amounts
* Models used:

  * XGBoost
  * Gradient Boosting
  * Baseline models

### Feature Importance

* Identification of key drivers influencing loan outcomes. 



## Usage

To run this project locally:

```bash
git clone <repository-url>
cd sba-analysis
```

Then:

1. Place the dataset in the appropriate directory
2. Open the Jupyter notebooks
3. Execute the analysis step by step

---

## Conclusion

This project illustrates how machine learning can enhance financial decision-making by identifying hidden risk patterns, improving lending strategies, and reducing exposure to loan defaults.

---
# Small Business Administration (SBA) Loan Analysis

## Overview

This project analyzes **U.S. Small Business Administration (SBA) loan data (1987–2014)** to uncover patterns in loan approvals, disbursements, and repayment outcomes.

The analysis integrates **data cleaning, exploratory data analysis (EDA), feature importance evaluation, and machine learning models** to generate actionable insights.

### Key Results

* **XGBoost** achieved the best classification performance:

  * ROC-AUC: 0.977
  * Accuracy: 94%
* **Gradient Boosting** produced the lowest RMSE for predicting loan approval amounts
* Key factors influencing repayment include:

  * Loan term
  * Bank affiliation
  * Industry type
  * Approved loan amount

This project demonstrates how **predictive analytics can support better lending decisions and reduce default risk**.

---

## Background

Small businesses play a significant role in:

* Economic growth
* Job creation
* Local development

Many rely on SBA-backed loans for startup capital, expansion, or recovery from financial challenges. The SBA guarantees a portion of these loans, reducing lender risk; however, defaults still result in financial losses.

### Loan Outcomes

* **PIF (Paid in Full):** Loan successfully repaid
* **CHGOFF (Charged Off):** Loan defaulted

Analyzing historical data helps identify risk patterns, borrower behavior, and predictive indicators of default.

---

## Research Problem

Despite the availability of large historical datasets, many lending decisions still rely on manual evaluation or broad rule-based systems. This approach often overlooks subtle but important patterns in the data.

This project addresses the following:

1. Identification of factors influencing loan repayment
2. Prediction of loan outcomes (PIF vs CHGOFF)
3. Modeling of key financial variables such as approval amounts
4. Development of data-driven decision support for lending

---

## Objectives

* Conduct exploratory analysis of SBA loan data
* Identify factors affecting loan repayment outcomes
* Develop classification models to predict loan status (PIF vs CHGOFF)
* Develop regression models to predict SBA-approved loan amounts

---

## Data Description

* **Source:** [https://pengdsci.github.io/datasets](https://pengdsci.github.io/datasets)
* **Period:** January 1987 – December 2014
* **Observations:** 899,164
* **Variables:** 27 (categorical and numerical)
* **Target Variable:** `MIS_Status`

The dataset includes borrower details, loan characteristics, bank information, and repayment outcomes.

### Notes

* The dataset contains historical formatting inconsistencies
* Only SBA-guaranteed loans are included

---

## Variable Summary

| Variable          | Type     | Description                      |
| ----------------- | -------- | -------------------------------- |
| LoanNr_ChkDgt     | Text     | Unique Loan Identifier           |
| Name              | Text     | Borrower Name                    |
| City              | Text     | Borrower City                    |
| State             | Text     | Borrower State                   |
| Zip               | Text     | Zip Code                         |
| Bank              | Text     | Lending Bank                     |
| BankState         | Text     | Bank Location                    |
| NAICS             | Text     | Industry Classification Code     |
| ApprovalDate      | Date     | Loan Approval Date               |
| ApprovalFY        | Text     | Fiscal Year                      |
| Term              | Numeric  | Loan Term (months)               |
| NoEmp             | Numeric  | Number of Employees              |
| NewExist          | Text     | 1 = Existing, 2 = New            |
| CreateJob         | Numeric  | Jobs Created                     |
| RetainedJob       | Numeric  | Jobs Retained                    |
| FranchiseCode     | Text     | Franchise Indicator              |
| UrbanRural        | Text     | 1 = Urban, 2 = Rural             |
| RevLineCr         | Text     | Revolving Credit Indicator (Y/N) |
| LowDoc            | Text     | LowDoc Program Indicator (Y/N)   |
| ChgOffDate        | Date     | Charge-Off Date                  |
| DisbursementDate  | Date     | Disbursement Date                |
| DisbursementGross | Currency | Amount Disbursed                 |
| BalanceGross      | Currency | Outstanding Balance              |
| MIS_Status        | Text     | Loan Status (Target Variable)    |
| ChgOffPrinGr      | Currency | Charged-Off Amount               |
| GrAppv            | Currency | Approved Loan Amount             |
| SBA_Appv          | Currency | SBA Guaranteed Amount            |

---

## Project Highlights

### Data Cleaning

* Handling missing values
* Standardizing inconsistent formats
* Cleaning categorical variables

### Exploratory Data Analysis

* Trends by year, industry, and geography
* Distribution of loan outcomes
* Identification of default patterns

### Predictive Modeling

* Classification: PIF vs CHGOFF
* Regression: Loan approval amounts
* Models used:

  * XGBoost
  * Gradient Boosting
  * Baseline models

### Feature Importance

* Identification of key drivers influencing loan outcomes. 



## Usage

To run this project locally:

```bash
git clone <repository-url>
cd sba-analysis
```

Then:

1. Place the dataset in the appropriate directory
2. Open the Jupyter notebooks
3. Execute the analysis step by step

---

## Conclusion

This project illustrates how machine learning can enhance financial decision-making by identifying hidden risk patterns, improving lending strategies, and reducing exposure to loan defaults.

---
