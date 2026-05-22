# 🚢 Titanic — Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=flat-square&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-4C72B0?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

> Analyze the Titanic passenger dataset to uncover survival patterns, key trends, and statistical insights through visualizations and structured reporting.

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Dataset Overview](#-dataset-overview)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Requirements](#-requirements)
- [How to Run](#-how-to-run)
- [Expected Output](#-expected-output)
- [Skills Demonstrated](#-skills-demonstrated)
- [License](#-license)

---

## 📖 About the Project

This project performs a full **Exploratory Data Analysis (EDA)** on the famous Titanic dataset. The goal is to understand what factors influenced passenger survival using:

- 📊 Statistical summaries
- 🔍 Missing value analysis
- 📈 Data visualizations (9 charts)
- 🔗 Correlation analysis
- 📋 Structured key findings report

---

## 🗂 Dataset Overview

| Property        | Details                          |
|----------------|----------------------------------|
| **Source**      | Seaborn built-in (`titanic`)     |
| **Rows**        | 891 passengers                   |
| **Columns**     | 15 features                      |
| **Target**      | `survived` (0 = No, 1 = Yes)    |

### Features Used

| Column     | Description                          |
|-----------|--------------------------------------|
| `survived` | Survival status (0 = No, 1 = Yes)   |
| `pclass`   | Passenger class (1st, 2nd, 3rd)     |
| `sex`      | Gender                               |
| `age`      | Age in years                         |
| `sibsp`    | # of siblings/spouses aboard         |
| `parch`    | # of parents/children aboard         |
| `fare`     | Ticket fare (£)                      |
| `embarked` | Port of embarkation (C, Q, S)       |

---

## 🔍 Key Findings

| Insight | Value |
|--------|-------|
| Overall Survival Rate | **38.4%** |
| Female Survival Rate | **74.2%** |
| Male Survival Rate | **18.9%** |
| 1st Class Survival | **63.0%** |
| 2nd Class Survival | **47.3%** |
| 3rd Class Survival | **24.2%** |
| Avg. Fare (Survivors) | **£48.40** |
| Avg. Fare (Non-Survivors) | **£22.12** |
| Avg. Age (Overall) | **29.7 years** |

### 💡 Main Conclusions

1. **"Women and children first"** — Female passengers had a survival rate nearly **4x higher** than males.
2. **Class inequality** — 1st class passengers were **2.6x more likely** to survive than 3rd class.
3. **Wealth mattered** — Survivors paid significantly higher fares on average.
4. **Passenger class** is the strongest numerical correlator with survival (`r = -0.338`).
5. **Age had minimal effect** — Survivors and non-survivors had similar average ages.

---

## 📊 Visualizations

The script generates a single comprehensive chart (`eda_titanic_report.png`) containing:

| # | Chart | Description |
|---|-------|-------------|
| 1 | Bar Chart | Survival Count |
| 2 | Grouped Bar | Survival by Sex |
| 3 | Grouped Bar | Survival by Passenger Class |
| 4 | Histogram | Age Distribution |
| 5 | KDE Plot | Age Distribution by Survival |
| 6 | Histogram | Fare Distribution |
| 7 | Heatmap | Survival Rate by Class & Sex |
| 8 | Grouped Bar | Survival by Embarkation Port |
| 9 | Correlation Heatmap | Numerical Feature Correlations |

---

## 📁 Project Structure

```
eda-titanic-project/
│
├── eda_titanic.py           # Main EDA script
├── eda_titanic_report.png   # Generated visualizations
└── README.md                # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have **Python 3.8+** installed.

```bash
python --version
```

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/eda-titanic-project.git
cd eda-titanic-project
```

---

## 📦 Requirements

Install all dependencies with:

```bash
pip install pandas numpy matplotlib seaborn
```

| Library      | Version  | Purpose                    |
|-------------|----------|----------------------------|
| `pandas`    | ≥ 2.0    | Data manipulation           |
| `numpy`     | ≥ 1.24   | Numerical operations        |
| `matplotlib`| ≥ 3.7    | Plotting & visualization    |
| `seaborn`   | ≥ 0.12   | Statistical visualizations  |

---

## ▶️ How to Run

```bash
python eda_titanic.py
```

The script will:
1. Load the Titanic dataset automatically (no download needed)
2. Print a full analysis report in the terminal
3. Save all charts to `eda_titanic_report.png` in the same folder

---

## ✅ Expected Output

**Terminal output includes:**
- Dataset shape & column info
- Statistical summary (numerical + categorical)
- Missing values report
- Survival rates by sex, class, age, and fare
- Correlation rankings

**File output:**
- `eda_titanic_report.png` — 9-panel visualization chart

---

## 🧠 Skills Demonstrated

- ✅ Data loading & inspection
- ✅ Handling missing values
- ✅ Descriptive statistics
- ✅ Data visualization (bar, histogram, KDE, heatmap)
- ✅ Correlation analysis
- ✅ Pattern recognition & insight extraction
- ✅ Structured reporting

---

## 📄 License

This project is licensed under the **MIT License** — free to use, modify, and distribute.

---

<div align="center">
  Made with 🐍 Python &nbsp;|&nbsp; Dataset via Seaborn
</div>
