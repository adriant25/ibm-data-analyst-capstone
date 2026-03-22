# Emerging Technology Trends: Insights from the Stack Overflow Developer Survey 2026

**IBM Data Analyst Professional Certificate — Capstone Project**

A data-driven analysis of the Stack Overflow Developer Survey to identify the most in-demand programming languages, databases, and platforms — both today and in the near future. Built as a portfolio project targeting a Data Analyst role.

> **Developer:** Jaiverth Adrian Tovar Lozada · Bogotá, Colombia

---

## Business Context

As an Associate Data Analyst at a global IT & business consulting firm, the goal is to provide stakeholders with evidence-based insights into the technology skills the market demands. This analysis answers:

1. Which programming languages are most in demand right now?
2. Which database technologies are most sought after?
3. Which IDEs dominate the developer ecosystem?
4. What technologies do developers want to learn next?
5. What do the demographics of the global developer community look like?

---

## Dataset

- **Source:** Stack Overflow Developer Survey (subset provided by IBM Skills Network)
- **Size:** 65,437 raw responses · 114 columns · 63,972 after cleaning
- **License:** [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/1-0/)

The dataset is loaded directly from the source URL — no manual download required.

---

## Analysis Pipeline

| Step | Task | Status |
|------|------|--------|
| 1 | Data Collection — load CSV, store in SQLite | ✅ Done |
| 2 | Data Exploration — shape, dtypes, descriptive stats | ✅ Done |
| 3 | Find & Remove Duplicates — 487 removed | ✅ Done |
| 4 | Handle Missing Values — median/mode imputation | ✅ Done |
| 5 | Normalize Data — Min-Max & Z-score on salary | ✅ Done |
| 6 | Feature Engineering — explode multi-value cols, `ExperienceLevel` | ✅ Done |
| 7 | Exploratory Data Analysis — distributions, IQR outliers, correlations | ✅ Done |
| 8 | Save Clean Dataset — CSV + SQLite export | ✅ Done |

---

## Key Findings

- **Python overtakes JavaScript** as the #1 desired language (34,245 vs 23,774) — driven by AI and data science demand
- **PostgreSQL dominates** both current use (40,232) and future demand (46,397) — the de facto relational standard
- **Swift commands the highest salary** ($130,801/yr); Python ranks 2nd ($114,383) — best ROI skill for data roles
- **25–34 age group** is the largest developer cohort; community is majority Junior/Mid experience
- **Job satisfaction correlates weakly with salary** — flexibility and culture matter more

---

## Repository Structure

```
├── data-collection/
│   ├── 01_Job_Data_API.ipynb                    # Fetch jobs.json, filter locally → xlsx
│   ├── 02_Popular_Languages_Scraping.ipynb      # Scrape HTML table → CSV
│   └── outputs/
│       ├── job-postings.xlsx                    # Job counts by city (7 cities)
│       ├── job-postings-technologies.xlsx       # Job counts by technology (12 techs)
│       └── popular-languages.csv               # Language salaries (10 languages)
├── capstone-project/
│   ├── Capstone_Survey_Analysis.ipynb           # Full 8-step analysis pipeline
│   ├── charts/                                  # 6 generated chart PNGs
│   ├── Presentation/
│   │   ├── capstone_v4.pptx                     # Final 20-slide presentation
│   │   └── Data Analyst Capstone Project.pdf    # PDF export
│   └── IBM Cognos Dashboard/
│       └── DashBoard IBM Course Project.pdf     # Interactive dashboard (PDF)
├── requirements.txt
└── README.md
```

---

## Deliverables

| Deliverable | Description |
|-------------|-------------|
| `Capstone_Survey_Analysis.ipynb` | Full 8-step analysis pipeline with findings on every step |
| `capstone_v4.pptx` | 20-slide presentation for stakeholders |
| `Data Analyst Capstone Project.pdf` | PDF export of the final presentation |
| `DashBoard IBM Course Project.pdf` | IBM Cognos Analytics dashboard (3 tabs) |
| `charts/` | 6 publication-ready chart PNGs |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Pandas](https://img.shields.io/badge/pandas-2.x-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-2.x-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-4c72b0)
![SQLite](https://img.shields.io/badge/SQLite-3.x-003B57?logo=sqlite)
![Jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626?logo=jupyter)

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/adriant25/ibm-data-analyst-capstone.git
cd ibm-data-analyst-capstone

# 2. Create and activate virtual environment
python -m venv .venv
# Windows PowerShell:
.venv\Scripts\Activate.ps1
# macOS / Linux:
source .venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run data collection (generates output files)
jupyter lab data-collection/01_Job_Data_API.ipynb
jupyter lab data-collection/02_Popular_Languages_Scraping.ipynb

# 5. Run the main analysis notebook
jupyter lab capstone-project/Capstone_Survey_Analysis.ipynb
```

Run all cells top-to-bottom. The main notebook downloads the survey dataset automatically on first run.

---

## Certificate

This project is part of the [IBM Data Analyst Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-analyst) on Coursera.
