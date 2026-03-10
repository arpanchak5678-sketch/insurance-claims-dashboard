# Insurance Claims Fraud & Risk Analytics Dashboard
**Tool:** Microsoft Excel | **Dataset:** 1,000 Auto Insurance Claims | **Domain:** BFSI

---

## Project Overview
An end-to-end Excel analytics project built on a real-world auto insurance claims dataset. The project covers the full analytics pipeline — raw data ingestion, cleaning, feature engineering, KPI reporting, pivot analysis, and an executive dashboard — mirroring workflows used in BFSI MIS and reporting roles.

---

## Workbook Structure (6 Sheets)

| Sheet | Purpose |
|---|---|
| `Raw_Data` | Original 1,000-record dataset with 39 fields (policy, incident, claim, fraud) |
| `Clean_Data` | Cleaned data with 7 engineered columns using advanced Excel formulas |
| `Analysis` | KPI summary sheet with key business metrics |
| `Pivots` | 5 pivot tables analysing claims across multiple dimensions |
| `Dashboards` | Visual dashboard with pivot charts for stakeholder reporting |
| `Insight` | 5 written business insights derived from the analysis |

---

## Key Features

### Data Cleaning & Feature Engineering
Added 7 calculated columns to the raw dataset:
- **`claim_year` / `claim_month`** — extracted using `YEAR()` and `TEXT()` for time-series analysis
- **`Sub_Claim_Total`** — sum of injury, property, and vehicle claims using `SUM()`
- **`claim_check`** — data validation flag comparing total vs sub-total to catch discrepancies
- **`Fraud_label`** — `IF()` formula converting Y/N to "Fraud" / "Not Fraud"
- **`Time_Category`** — nested `IF()` bucketing incident hour into Night / Morning / Afternoon / Evening
- **`Severity_Risk`** — `VLOOKUP()` mapping incident severity to risk level (No Risk → High Risk)

### KPI Summary (Analysis Sheet)
| Metric | Formula Used |
|---|---|
| Total Claim Exposure | `SUM` |
| Average Claim Value | `AVERAGE` |
| Maximum Single Claim | `MAX` |
| Total Fraud Cases | `COUNTIF` |
| Fraud Rate | `COUNTIF / COUNTA` |

### Pivot Table Analysis (5 Tables)
- Claim amount by **incident type**
- Fraud distribution by **state** (IL, IN, OH)
- Claim cost by **vehicle brand**
- Accidents by **time of day**
- Claim cost by **incident severity**

---

## Key Findings

- **24.7% fraud rate** — 247 of 1,000 claims flagged as fraudulent
- **Multi-vehicle and single-vehicle collisions** account for the largest share of total claim payouts (~$52.7M combined)
- **Evening hours** record the highest accident frequency — likely driven by peak commute traffic
- **Major, Minor, and Total Loss** severity tiers contribute near-equal claim costs (~$17M each), suggesting severity alone isn't the primary cost driver
- **Dodge, Subaru, and Saab** generate the highest brand-level claim costs; Honda the lowest

---

## Skills Demonstrated
`Advanced Excel` `Nested IF` `VLOOKUP` `XLOOKUP` `INDEX-MATCH` `COUNTIF` `TEXT` `YEAR` `Data Validation` `Pivot Tables` `Pivot Charts` `KPI Dashboards` `BFSI Domain Knowledge` `Data Cleaning` `Feature Engineering`

---

## About
Built as a self-initiated project to demonstrate applied Excel analytics skills in an insurance context, directly aligned with MIS Analyst and Junior Data Analyst roles in the BFSI sector.

**Author:** Arpan Chakraborty  
**LinkedIn:** [linkedin.com/in/arpan-chakraborty-603755251](https://www.linkedin.com/in/arpan-chakraborty-603755251)
