# Emerging Technology Trends: Insights from the Stack Overflow Developer Survey

**IBM Data Analyst Professional Certificate — Capstone Project**

A data-driven analysis of the Stack Overflow Developer Survey to identify the most in-demand programming languages, databases, and platforms — both today and in the near future. Built as a portfolio project targeting a Data Analyst role.

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
- **Size:** 65,000+ responses, 114 columns
- **License:** [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/1-0/)

The dataset is loaded directly from the source URL — no manual download required. See the notebook for details.

---

## Project Pipeline

| Step | Task | Status |
|------|------|--------|
| 1 | Data Collection — load CSV, store in SQLite | ✅ Done |
| 2 | Data Exploration — shape, dtypes, descriptive stats | 🔄 In Progress |
| 3 | Find & Remove Duplicates | ⏳ Pending |
| 4 | Handle Missing Values — median/mode imputation | ⏳ Pending |
| 5 | Normalize Data — Min-Max & Z-score normalization | ⏳ Pending |
| 6 | Feature Engineering — explode multi-value columns, create `ExperienceLevel` | ⏳ Pending |
| 7 | Exploratory Data Analysis — distributions, outliers, correlations | ⏳ Pending |
| 8 | Save Clean Dataset | ⏳ Pending |

---

## Repository Structure

```
├── capstone-project/
│   ├── Capstone_Survey_Analysis.ipynb   # Main analysis notebook (Steps 1–8)
│   └── capstone_v2.pptx                 # Final presentation deck
└── lab_codes_practice/                  # 23 practice notebooks (one per topic)
    ├── Data Collection
    ├── Data Wrangling
    ├── Exploratory Data Analysis
    └── Data Visualization
```

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Pandas](https://img.shields.io/badge/pandas-2.x-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-1.x-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-4c72b0)
![SQLite](https://img.shields.io/badge/SQLite-3.x-003B57?logo=sqlite)
![Jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626?logo=jupyter)

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/ibm-data-analyst-capstone.git
cd ibm-data-analyst-capstone

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn openpyxl requests jupyter

# 3. Open the main notebook
jupyter lab capstone-project/Capstone_Survey_Analysis.ipynb
```

Run cells from top to bottom. The notebook downloads the dataset automatically on first run.

---

## Certificate

This project is part of the [IBM Data Analyst Professional Certificate](https://www.coursera.org/professional-certificates/ibm-data-analyst) on Coursera.
