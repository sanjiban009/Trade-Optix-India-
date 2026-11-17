# TradeOptix India
## FMCG Trade Promotion Optimization & Profitability Intelligence

**Portfolio case study by Sanjiban Das** · Indian FYTD (April–March) · Power BI-style HTML dashboard · Excel + CSV data model

<img width="1512" height="1447" alt="01_Executive_Overview" src="https://github.com/user-attachments/assets/42a1bf3f-5390-4883-b575-1c78425d367e" />


> **Synthetic data notice:** Every brand, transaction, distributor, retailer, promotional scheme, claim, KPI, scenario result and financial amount in this project is fictitious. It is a realistic demonstration, not a report on any actual company or verified operational achievement. Causal uplift and baseline assumptions have not been validated with real controls.

### Quick start

1. Download and extract the release ZIP (do not open files from inside the compressed archive).
2. Double-click **`OPEN_DASHBOARD.html`** or **`dashboard/index.html`**.
3. Navigate all eight dashboard pages using the sidebar.
4. Select fiscal year, period, region, product category, channel and scheme type.
5. Use **Export Filtered CSV** for the currently selected scheme records.
6. Open **Methodology** for definitions, reporting constraints and how the synthetic model works.

**Offline-first:** no installation, login, backend, API key, CDN, Python, Node or internet connection is required to run the dashboard locally. `dashboard/dataset.js` includes the complete 960-row scheme-level analytics model; transaction-level detail is in `/data/*.csv`.

### Eight interactive pages

| # | Analytics page | Business decision |
| --- | --- | --- |
| 1 | Executive Command Center | Which trade schemes create positive incremental net impact? |
| 2 | Scheme Planning & Budgets | Which budgets are overspent or under-utilized? |
| 3 | Primary vs Secondary Sales | Is sell-in moving faster than sell-through? |
| 4 | Promotional Uplift | What is the estimated baseline-adjusted incremental volume? |
| 5 | Promotion ROI & Margin | Which schemes cover their total cost? |
| 6 | Distributor & Retailer | Which regions and channels deserve closer commercial review? |
| 7 | Claims & Scheme Leakage | What claims need reconciliation and what settlements remain outstanding? |
| 8 | Promotion Optimizer | How sensitive is incremental profit to uplift, discount and budget assumptions? |

### Interactive features

- Indian **FY 2025–26** and **FY 2026–27**, fiscal quarters, FYTD, full-data selection, Oct–Nov comparison.
- Six global slicers affecting every page, KPI, chart, ranking and intelligence insight.
- 8 unique management views, interactive SVG charts with browser hover values, financial tables and exception views.
- Dynamic business-intelligence highlight cards updated with each filter change.
- Scheme-level CSV export, cost and profitability diagnostics, forecast sensitivity controls.
- Accessible navigation, responsive layouts and no network dependencies.

### Data structure

| File | Description | Records |
| --- | --- | ---: |
| `data/Promotion_Master.csv` | Promotion scope and scheme terms | 960 |
| `data/Scheme_Fact_Model.csv` | Joined analytics record per scheme | 960 |
| `data/Primary_Sales.csv` | Manufacturer-to-distributor order lines | 3,840 |
| `data/Secondary_Sales.csv` | Distributor-to-retailer invoice lines | 19,200 |
| `data/Promotion_Claims.csv` | Claim submissions and settlement | 960 |
| `data/Distributor_Inventory.csv` | Inventory stock bridges | 960 |
| `data/Trade_Budget.csv` | Scheme budgets and variance | 960 |
| `data/Baseline_Demand.csv` | Estimated counterfactual unit demand | 960 |
| `data/Distributor_Master.csv` | Fictional distribution partners | 60 |
| `data/Retailer_Master.csv` | Fictional retail outlets | 840 |
| `data/Product_Master.csv` | Fictional FMCG SKU catalog | 12 |
| `data/Fiscal_Calendar.csv` | Monthly Indian financial calendar | 20 |
| `data/TradeOptix_Excel_Data_Model.xlsx` | Multi-sheet Excel model and calculated KPIs | 9 sheets |

The scope is intentionally a compact **demonstration**, not a claim to represent a complete national FMCG manufacturer's ERP system.

### Model definitions

- **Gross uplift %:** `(Actual secondary units − Estimated baseline units) / Baseline units × 100`.
- **Adjusted incremental units:** `Secondary − Baseline − Estimated cannibalization`.
- **Incremental contribution:** `Adjusted incremental units × illustrative unit contribution`.
- **Net incremental impact:** `Incremental contribution − (trade spending + execution costs)`.
- **Promotion ROI:** `Net incremental impact / total promotion cost × 100`.
- **Claim settlement outstanding:** `Approved claim − Paid claim`.
- **Primary-secondary volume gap:** `Primary units − Secondary units`. A gap alone does *not* establish channel stuffing.

The synthetic baseline does not establish a causal effect. A real production model would include promoted and non-promoted control groups, comparable stores, seasonality, stockouts, implementation lags, returns, and external conditions. Actual GST accounting may differ by trade scheme and must be validated separately.

**Tech Stack:** HTML5 | CSS3 | JavaScript | Advanced Excel | CSV | JSON | Business Intelligence | Data Visualization | KPI Modeling | Financial Analytics | 

### Suggested project skills

Commercial Analytics · FMCG Trade Promotion Management (TPM) · Trade Promotion Optimization (TPO) · FYTD · Budget Variance · Primary & Secondary Sales · Distributor Analytics · Profitability · HTML · CSS · JavaScript · Excel · Financial Modelling · Data Visualization · Decision Intelligence

### License & usage

Open-source demonstration under the MIT License. Please preserve the synthetic data disclosure in any redistribution. See `LICENSE`.
<img width="1512" height="1458" alt="04_Promotion_Optimizer" src="https://github.com/user-attachments/assets/3b7d9f28-cc37-49fa-8c6e-5be48e532999" />
<img width="1512" height="1687" alt="03_Promotion_ROI" src="https://github.com/user-attachments/assets/452973f1-3198-4a39-90e7-c4f8d27b16c2" />
<img width="1512" height="1405" alt="02_Primary_Secondary" src="https://github.com/user-attachments/assets/de1cb68f-989c-4c0b-8e97-61fe9940b6f6" />
<img width="1512" height="1447" alt="01_Executive_Overview" src="https://github.com/user-attachments/assets/42e73a67-6a9a-4052-8ae6-617a82990ff6" />



