# 🏦 NovaBridge Bank Nigeria — Transaction & Portfolio Analysis
### DataBeginners Week 4 Project | Built with Microsoft Excel

---

## 📌 Project Overview

This project delivers a **two-page interactive Excel dashboard** for **NovaBridge Bank Nigeria** — a fictional tier-2 commercial bank operating **10 branches** across **5 geopolitical zones** in Nigeria. The analysis covers **1,050 transaction records** from 2023 to 2024 calendar year spanning **334 unique customers** and **375 unique accounts**.

This project was completed as part of the **DataBeginners Week 4 curriculum** — a WhatsApp-based data analytics learning community — and represents the first end-to-end banking analytics project in my portfolio built entirely in Microsoft Excel using Pivot Tables, SUMIFS, VLOOKUP, data cleaning and interactive dashboard design.

---

## ❓ Business Problem Statement

> *"NovaBridge Bank Nigeria operates 10 branches across 5 geopolitical zones serving 334 unique customers across Retail, SME, Corporate and Premium segments. In 2024 the bank processed 1,050 transactions totalling ₦1.70 billion in NGN-denominated value — but management has limited visibility into the underlying patterns driving that performance.*
>
> *The bank does not know which branches are truly leading transaction value, whether its digital channels are growing, which customer segments are most profitable, how its loan portfolio risk is distributed, or why 11.7% of all transactions are failing. Additionally, the bank's loan pricing does not appear to reflect individual borrower creditworthiness — creating potential risk-pricing mismatches in its largest lending categories.*
>
> *A data analyst has been engaged to clean the raw transaction data, investigate data quality issues, uncover key performance patterns across commercial and risk dimensions, and deliver a two-page interactive Excel dashboard that answers the bank's 10 most pressing business questions with actionable recommendations."*

---

## 📊 Dashboard Preview

### Page 1 — Transaction & Customer Segment Overview
![Transaction Overview](assets/Page%201.png)

### Page 2 — Risk & Loan Portfolio Analysis
![Risk and Loan Analysis](assets/Page%202.png)

---

## 🔍 Insight Questions

### Page 1 — Transaction & Customer Overview
1. Which of the 10 branches generated the highest total transaction value in 2024?
2. What percentage of transactions came through each digital channel — and which channel leads adoption?
3. What is the proportion of Deposits versus Withdrawals — is NovaBridge experiencing a net inflow or outflow?
4. Which customer segment (Retail, SME, Corporate or Premium) contributes the most total transaction value?
5. Which day of the week has the highest transaction volume — and what does this mean for operational planning?
6. How did monthly transaction values trend across 2024 — which month was the strongest and weakest?

### Page 2 — Risk & Loan Portfolio Analysis
7. What is the breakdown of transactions by Risk Rating — and which risk category generates the most failures?
8. Which loan purpose carries the largest portfolio value — and which has the highest credit risk?
9. Is there a relationship between loan purpose, interest rate and borrower credit score?
10. Which Relationship Manager manages the highest total transaction value?

---

## 💡 Key Findings

---

### Commercial & Branch Performance

**Finding 1 — Abuja Main Dominates Branch Performance**
Abuja Main generated the highest transaction value at **₦19.46M** — 7.6x more than
the lowest branch Warri at ₦2.55M. Lagos Island follows at ₦16.60M and Port Harcourt
at ₦15.18M. The wide performance gap between Abuja Main and Warri suggests a
significant customer acquisition or service capacity disparity that demands branch-level
investigation.

**Finding 2 — Mobile App Leads Digital Adoption at 32.45%**
Mobile App accounts for **32.45% of all transactions** — the highest of any channel.
ATM follows at 26.00% and Branch at 17.79%. USSD — typically serving lower-income
and rural customers — accounts for only 2.54%. NovaBridge's customer base is
smartphone-first, confirming digital infrastructure investment should prioritise
mobile experience over branch or USSD capability.

**Finding 3 — NovaBridge is in Net Inflow Position**
Deposits at **₦45.78M** lead all transaction types in value, followed by Transfer In
at ₦22.19M. Withdrawals (₦11.36M) and Transfer Out (₦13.38M) are significantly
lower — confirming more money is flowing into the bank than leaving. This is a
positive liquidity signal that management should monitor quarterly.

**Finding 4 — SME and Retail Drive 71.3% of Transaction Value**
SME (35.39%) and Retail (35.89%) together account for **71.28%** of total NGN
transaction value. Corporate and Premium combined contribute only 28.71% despite
Premium customers typically representing the bank's highest-net-worth individuals.
This underperformance from the top two segments represents a commercial gap —
either Premium customers are under-transacting or routing higher-value business
through competitor banks.

**Finding 5 — Monday is the Busiest Transaction Day**
Monday leads weekly transaction volume at **162 transactions**, declining steadily
through the week to Sunday at 136. This front-loaded weekly pattern has direct
implications for branch staffing, digital channel capacity and customer support
scheduling — with Monday requiring the most operational resources of any day.

**Finding 6 — 5 Outlier Transactions Require Management Investigation**
Four customers — Fatima Okafor (₦493.09M), Ibrahim Okafor (₦407.27M),
Haliru Obi (₦357.51M combined across 2 transactions) and Emeka Nnaji (₦335.68M)
— generated transactions statistically abnormal relative to the full dataset.
Three of these five events occurred in June, directly driving an anomalous monthly
spike. These were isolated in a dedicated Outlier Review table and **excluded from
all KPI totals** pending management investigation under AML protocols.

---

### Risk & Loan Portfolio

**Finding 7 — Low Risk Customers Generate the Most Failed Transactions**
Counterintuitively Low risk customers generated **48 failed transactions** — the
highest of any risk category — while High risk customers generated only 10 and
Medium risk generated 59 across a larger base. This confirms that transaction
failures in NovaBridge's system are driven by **operational and technical causes**
(insufficient funds, network failures, duplicate blocks) rather than customer
risk profile. The risk classification system is functioning correctly for credit
assessment but a separate operational failure investigation is urgently needed.

**Finding 8 — Agriculture is the Largest but Riskiest Loan Exposure**
Agriculture has the largest loan portfolio at **₦994.61M** — the bank's single
biggest lending concentration — but Agriculture borrowers carry the **lowest
average credit score at 540.36**. Despite this weak borrower profile, Agriculture
receives the second cheapest average interest rate at 20.49%. The bank is holding
its highest loan concentration in its weakest borrower segment at a below-market
price — a textbook risk-pricing mismatch.

**Finding 9 — Equipment Borrowers Are Overcharged Relative to Their Credit Profile**
Equipment loan customers have the strongest average credit score in the portfolio
at **614.09** — the best borrower quality of any loan category — but are charged
the second highest interest rate at **22.47%**. The bank's strongest borrowers are
paying near-premium rates. This misalignment risks pushing high-quality Equipment
customers to seek better-priced lending from competitor banks.

**Finding 10 — Loan Pricing Follows Product Category, Not Creditworthiness**
The correlation between Credit Score and Interest Rate across the loan book is
**effectively zero (r = 0.031)**. Interest rates are set by loan purpose category
not individual borrower creditworthiness. This means NovaBridge is not operating
a risk-based pricing model — it is applying standardised product rates regardless
of how strong or weak each individual borrower's credit profile is.

**Finding 11 — 10 Customers Have No Risk Rating**
10 transactions belong to customers with no Risk Rating recorded — meaning these
accounts were activated or transacted without a completed risk classification.
This represents a compliance gap against CBN AML/CFT requirements which mandate
risk classification for all active bank customers.

**Finding 12 — Tunde Ojo Leads RM Performance with a Significant Gap**
Tunde Ojo manages the highest portfolio value at **₦15.00M** — nearly double
Bello Usman at ₦8.27M. A gap this wide is unlikely to reflect skill alone and
more probably reflects unequal portfolio allocation — creating concentration risk
in Tunde Ojo's book and underdevelopment in lower-performing RMs.

---

## ✅ Recommendations

**Recommendation 1 — Investigate and Escalate the 5 Outlier Transactions**
The four flagged customers generated transactions statistically inconsistent with
the full portfolio. These should be reviewed under NovaBridge's AML/transaction
monitoring framework immediately. Haliru Obi appearing twice is particularly notable.
Until investigation is complete these transactions should remain excluded from
all strategic revenue and volume planning figures.

**Recommendation 2 — Launch a Branch Recovery Plan for Warri**
At ₦2.55M, Warri generates less than 14% of Abuja Main's value from a market
that should be commercially viable. A root cause review covering customer acquisition,
product availability, local competition and branch capacity should be commissioned
with quarterly improvement targets set and tied to branch management accountability.

**Recommendation 3 — Prioritise Mobile App Investment as the Primary Channel**
With 32.45% of transactions already on Mobile App and USSD at only 2.54%,
NovaBridge's customers are smartphone-first. Product and technology investment
should prioritise Mobile App feature development — particularly for higher-value
services like loan applications, fixed deposit placements and large transfers —
over USSD or physical branch infrastructure.

**Recommendation 4 — Implement Risk-Based Pricing for Agriculture Loans**
The Agriculture portfolio is ₦994.61M with the weakest borrower credit profile
(540.36 avg score) at below-average pricing (20.49% avg rate). The Credit team
should model the impact of raising Agriculture loan rates by 100-150 basis points
to reflect actual borrower risk. This adjustment on the bank's largest loan
category would materially improve net interest margin with no new lending required.

**Recommendation 5 — Reward Strong Equipment Borrowers with Rate Relief**
Equipment borrowers have the portfolio's strongest credit profiles (614.09 avg
score) but pay near-premium rates (22.47%). Offering rate reductions of 50-100
basis points to Equipment borrowers with credit scores above 650 would improve
retention of the bank's highest-quality lending customers — who are most likely
actively comparing rates across lenders.

**Recommendation 6 — Resolve All 10 Unclassified Risk Ratings Within 30 Days**
The 10 Not Rated accounts represent a CBN compliance gap. The Risk and Compliance
team should complete these classifications within 30 days and audit the customer
onboarding process to identify and close the procedural gap that allowed these
accounts to become active without a completed risk profile.

**Recommendation 7 — Investigate Operational Transaction Failure Causes**
The 11.7% failed transaction rate concentrated among Low risk customers confirms
failures are operational not credit-driven. A technical investigation into the
top failure reasons — insufficient funds flagging, network timeouts, duplicate
transaction blocks — should be conducted immediately. Reducing the failure rate
from 11.7% to below 5% would directly improve customer experience and recover
lost transaction fee revenue.

**Recommendation 8 — Rebalance RM Portfolio Allocation**
The gap between Tunde Ojo (₦15M) and Bello Usman (₦8.27M) is too wide to reflect
skill alone. A portfolio rebalancing exercise — redistributing Corporate and Premium
segment accounts more equitably — would develop team-wide capability, reduce
single-RM concentration risk and give junior RMs the exposure needed to grow their
performance to Tunde Ojo's level.

---

## ⚠️ Data Quality Issues Found & Fixed

| Issue | Detail | Fix Applied |
|---|---|---|
| Inconsistent Account_Type | 10 variants for 5 types (e.g. SAV, loan, FD) | Find & Replace — standardised to 5 clean values |
| Inconsistent Status | 7 variants (Successfull, success, FAILED) | Find & Replace — standardised to 4 values |
| Inconsistent Channel | 12 variants + 9 blanks | Find & Replace + blanks filled with "Unknown" |
| Inconsistent Branch | Case inconsistency across 10 branches | Find & Replace — standardised to Title Case |
| Duplicate Transaction IDs | 18 duplicate records found | Removed via Data → Remove Duplicates |
| Foreign Currency Mix | 309 USD/GBP rows in NGN column | Separated — NGN used for KPIs, FX shown separately |
| Amount Outliers >₦80M | 5 transactions statistically abnormal | Isolated in Outlier Review table, excluded from KPI totals |
| Missing Relationship_Manager | 6 blank values | Filled with "Unassigned" |
| Missing Region | 8 blank values | Filled via VLOOKUP from Branch Reference sheet |
| Missing Risk_Rating | 10 blank values | Filled with "Not Rated" |
| Missing Occupation | 7 blank values | Filled with "Not Stated" |
| Missing Channel | 9 blank values | Filled with "Unknown" |

---

## 🗄️ Dataset Information

| Field | Detail |
|---|---|
| Source | DataBeginners Week 4 — NovaBridge Bank Nigeria Dataset |
| Total Records | 1,050 transactions |
| Unique Customers | 334 |
| Unique Accounts | 375 |
| Branches | 10 across 5 geopolitical zones |
| Date Range | January 2024 — December 2024 |
| Currencies | NGN (741), USD (174), GBP (135) |

### Column Reference

| Column | Description |
|---|---|
| Transaction_ID | Unique transaction identifier |
| Date / Month / Quarter / Day_of_Week | Transaction timing fields |
| Customer_Name / Customer_ID | Customer identification |
| Account_Number / Account_Type | Account details |
| Transaction_Type | Deposit, Withdrawal, Transfer In/Out, POS, Loan Repayment |
| Amount_NGN | Transaction value (note: FX rows stored in original currency) |
| Currency | NGN, USD or GBP |
| Status | Successful, Failed, Pending, Reversed |
| Branch / Region | Branch name and geopolitical zone |
| Channel | Mobile App, ATM, Branch, Online Banking, POS, USSD |
| Customer_Segment | Retail, SME, Corporate, Premium |
| Risk_Rating | High, Medium, Low, Not Rated |
| Credit_Score | 300-850 scale (loan customers only) |
| Loan_Amount_NGN | Loan facility value |
| Interest_Rate_Pct | Annual loan interest rate |
| Loan_Purpose | Agriculture, Business Capital, Education, Equipment, Home Purchase, Personal, Vehicle Purchase |
| Loan_Tenor_Months | Loan repayment duration |
| Relationship_Manager | Assigned RM name |
| Occupation | Customer's stated occupation |

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data cleaning, analysis and dashboard |
| Pivot Tables | All chart data aggregation |
| SUMIFS / COUNTIFS / AVERAGEIF | KPI calculations |
| VLOOKUP | Filling missing Region from Branch Reference |
| Custom Number Formats | ₦B and ₦M display formatting |
| Find & Replace | Data standardisation |
| Slicers | Interactive dashboard filtering |

---

## 👤 About the Analyst

**Fatimah Ojuolape Olatunji**
Data Analyst | DataBeginners Community Founder & Lead Mentor
Obafemi Awolowo University (OAU) | Final Year Business Administration

This project is part of my public analytics learning journey and was built
as a teaching resource for the **DataBeginners WhatsApp learning community**
— where I mentor aspiring analysts through weekly hands-on Excel and Power BI
projects from raw dataset to completed dashboard.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin)](YOUR_LINKEDIN_URL)
[![Twitter](https://img.shields.io/badge/Twitter-Follow-1DA1F2?style=flat&logo=twitter)](https://twitter.com/ojuolape124)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-181717?style=flat&logo=github)](https://github.com/ojuolape124)

---

*This project was built as Week 4 of the DataBeginners curriculum — covering
data cleaning, Pivot Table analysis, VLOOKUP, custom number formatting and
two-page Excel dashboard design. Every step was documented and taught live
in the DataBeginners WhatsApp community.*
