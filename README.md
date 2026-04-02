# NST DVA Capstone 2 — Project Repository

> **Newton School of Technology | Data Visualization & Analytics**
> A 3-week industry-simulation capstone using Python, GitHub, and Tableau to convert raw data into actionable business intelligence.

---

## Project Overview

|       Field         |                 Details                     |
|---------------------|---------------------------------------------|
| **Project Title**   | _To be filled by team_                      |
| **Sector**          | _e.g., Retail, Finance, Healthcare, EdTech_ |
| **Team ID**         | _e.g., DVA-B1-T3_                           |
| **Section**         | _To be filled by team_                      |
| **Faculty Mentor**  | _To be filled by team_                      |
| **Institute**       | Newton School of Technology                 |
| **Submission Date** | _To be filled by team_                      |

### Team Members

|       Role         |     Name         | GitHub Username |
|--------------------|------------------|-----------------|
| Project Lead       |------------------|-----------------|
| Data Lead          |------------------|-----------------|
| ETL Lead           |------------------|-----------------|
| Analysis Lead      |------------------|-----------------|
| Visualization Lead |------------------|-----------------|
| Strategy Lead      |------------------|-----------------|
| PPT & Quality Lead |------------------|-----------------|

---

## Business Problem

_Describe the sector context, the decision-maker this project serves, and the core business challenge being addressed. Keep this to 3–5 sentences written in plain language, as if addressing a senior stakeholder._

**Core Business Question:**
> _State the single main question your Tableau dashboard and Python analysis will answer._

**Decision Supported:**
> _What action or decision will this analysis enable the stakeholder to take?_

---

## Dataset

|                    Attribute                          |                    Details                         |
|-------------------------------------------------------|----------------------------------------------------|
| **Source Name**                                       | _e.g., World Bank, data.gov.in, Kaggle (raw only)_ |
| **Direct Access Link**                                | _Paste the direct download or access URL_          |
| **Row Count**                                         | _Must be > 5,000_                                  |                                
| **Column Count**                                      | _Must be > 8 meaningful columns_                   |
| **Time Period Covered**                               | _e.g., Jan 2019 – Dec 2023_                        |
| **Format**                                            | _e.g., CSV, JSON, Excel_                           |

**Key Columns Used:**

| Column Name | Description | Role in Analysis |
|-------------|-------------|------------------|
|-------------|-------------|------------------|
|-------------|-------------|------------------|
|-------------|-------------|------------------|
|-------------|-------------|------------------|
|-------------|-------------|------------------|
|-------------|-------------|------------------|


For full column definitions, see [`docs/data_dictionary.md`](docs/data_dictionary.md).

---

## KPI Framework

| KPI | Definition | Formula / Computation |
|---|---|---|
| _e.g., Monthly Revenue Growth %_ | | See `notebooks/04_statistical_analysis.ipynb` |
| _e.g., Customer Churn Rate_ | | See `notebooks/04_statistical_analysis.ipynb` |

---

## Tableau Dashboard

|           Item       |                     Details                |
|----------------------|--------------------------------------------|
| **Dashboard URL**    | _Paste Tableau Public link here_           |
| **Executive View**   | _Describe the high-level KPI summary view_ |
| **Operational View** | _Describe the detailed drill-down view_    |

Screenshots are available in [`tableau/screenshots/`](tableau/screenshots/). The full public URL is also documented in [`tableau/dashboard_links.md`](tableau/dashboard_links.md).

---

## Key Insights

_List 8–12 major findings from the analysis, written in decision language. Each insight should tell the reader what to think or act upon — not merely describe a chart._

1.
2.
3.
4.
5.
6.
7.
8.

---

## Recommendations

_Provide 3–5 specific, actionable business recommendations, each linked directly to an insight above._

| # | Insight | Recommendation | Expected Impact |
|---|---------|--------------|-------------------|
| 1 |---------|--------------|-------------------|
| 2 |---------|--------------|-------------------|
| 3 |---------|--------------|-------------------|

---

## Repository Structure

```
SectionName_TeamID_ProjectName/
│
├── README.md                          ← This file
│
├── data/
│   ├── raw/                           ← Original dataset (never edited)
│   └── processed/                     ← Cleaned output from ETL pipeline
│
├── notebooks/
│   ├── 01_extraction.ipynb            ← Data sourcing and initial load
│   ├── 02_cleaning.ipynb              ← Python ETL and cleaning pipeline
│   ├── 03_eda.ipynb                   ← Exploratory data analysis
│   ├── 04_statistical_analysis.ipynb  ← Forecasting, regression, hypothesis testing
│   └── 05_final_load_prep.ipynb       ← KPI computation and final data prep
│
├── scripts/
│   └── etl_pipeline.py                ← Reusable ETL pipeline script
│
├── tableau/
│   ├── screenshots/                   ← Dashboard screenshots (PNG)
│   └── dashboard_links.md             ← Tableau Public URL
│
├── reports/
│   ├── project_report.pdf             ← Final academic + industry report (10–15 pages)
│   └── presentation.pdf              ← Final presentation deck (10–12 slides)
│
├── docs/
│   └── data_dictionary.md             ← Full column definitions and data notes
│
├── DVA-oriented-Resume/               ← Individual DVA-focused resumes
└── DVA-focused-Portfolio/             ← Individual portfolio references
```

---

## Analytical Pipeline

The project follows a structured 7-step workflow:

1. **Define** — Sector selected, problem statement scoped, mentor approval obtained (Gate 1)
2. **Extract** — Raw dataset sourced and committed to `data/raw/`; data dictionary drafted
3. **Clean & Transform** — Python ETL pipeline built in `notebooks/02_cleaning.ipynb`; all steps logged
4. **Analyze** — EDA and statistical analysis performed in notebooks 03 and 04
5. **Visualize** — Interactive Tableau dashboard built and published on Tableau Public
6. **Recommend** — 3–5 data-backed business recommendations delivered
7. **Report** — Final project report and presentation deck completed and committed

---

## Tech Stack

| Tool | Status | Purpose |
|---|---|---|
| Python + Jupyter Notebooks | Mandatory | All ETL, cleaning, and statistical analysis |
| Google Colab | Supported | Notebook execution environment (`.ipynb` committed to GitHub) |
| Tableau Public | Mandatory | Dashboard design, publishing, and sharing |
| GitHub | Mandatory | Version control, collaboration, contribution audit |
| SQL | Optional | Initial data extraction only (if used, documented in repo) |

**Key Python libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`

---

## Evaluation Rubric

| Area | Marks | Focus |
|---|---|---|
| Problem Framing | 10 | Is the business question clear and well-scoped? |
| Data Quality & ETL | 15 | Is the Python pipeline thorough and documented? |
| Analysis Depth | 25 | Are statistical methods applied correctly with insight? |
| Dashboard & Visualization | 20 | Is the Tableau dashboard interactive and decision-relevant? |
| Business Recommendations | 20 | Are insights actionable and well-reasoned? |
| Storytelling & Clarity | 10 | Is the presentation professional and coherent? |
| **Total** | **100** | |

> Marks are awarded for analytical thinking and decision relevance — not chart quantity, visual decoration, or code length.

---

## Submission Checklist

**GitHub Repository**
- [ ] Public repository created with the correct naming convention (`SectionName_TeamID_ProjectName`)
- [ ] All notebooks committed in `.ipynb` format
- [ ] `data/raw/` contains the original, unedited dataset
- [ ] `data/processed/` contains the cleaned pipeline output
- [ ] `tableau/screenshots/` contains dashboard screenshots
- [ ] `tableau/dashboard_links.md` contains the Tableau Public URL
- [ ] `docs/data_dictionary.md` is complete
- [ ] `README.md` explains the project, dataset, and team
- [ ] All members have visible commits and pull requests

**Tableau Dashboard**
- [ ] Published on Tableau Public and accessible via public URL
- [ ] At least one interactive filter included
- [ ] Dashboard directly addresses the business problem

**Project Report (PDF, 10–15 pages)**
- [ ] Cover page, executive summary, sector context, problem statement
- [ ] Data description, cleaning methodology, KPI framework
- [ ] EDA with written insights, statistical analysis results
- [ ] Dashboard screenshots and explanation
- [ ] 8–12 key insights in decision language
- [ ] 3–5 actionable recommendations with impact estimates
- [ ] Contribution matrix (must match GitHub history)

**Presentation Deck (PDF, 10–12 slides)**
- [ ] Title slide through Recommendations, Impact, Limitations, and Next Steps

**Individual Assets**
- [ ] DVA-oriented Resume updated to include this capstone
- [ ] Portfolio link shared (if applicable)

---

## Contribution Matrix

This table must match evidence in GitHub Insights, PR history, and committed files.

| Team Member | Dataset & Sourcing | ETL & Cleaning | EDA & Analysis | Statistical Analysis | Tableau Dashboard | Report Writing | PPT & Viva |
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|
|-------------|--------------------|----------------|----------------|-----------------------|------------------|----------------|------------|


_Declaration: We confirm that the above contribution details are accurate and verifiable through GitHub Insights, PR history, and submitted artifacts._

**Team Lead Name:** _____________________________ **Date:** _______________

---

## Academic Integrity

All analysis, code, and recommendations in this repository are the original work of the team listed above. Free-riding is tracked via GitHub Insights and PR history. Any mismatch between the contribution matrix and actual commit history may result in individual grade adjustments.

---

*Newton School of Technology — Data Visualization & Analytics | Capstone 2*