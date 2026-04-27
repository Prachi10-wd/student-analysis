# 🎓 Student Performance Analysis
### Does your parent's education affect your grades? The data has something to say.
---

## 📌 Project Overview

This is my **first end-to-end data analysis project** — a complete Python workflow from raw Kaggle data to cleaned insights and visualizations.

The central question: **Does parental education level influence student grades?**

Spoiler: The 7-point gap is real. But the *interpretation* is where real analysis begins.

---

## 🔧 Workflow

```
Raw Data (Kaggle)
      ↓
Pre-Cleaning Audit
      ↓
Data Cleaning & Feature Engineering
      ↓
Visualization & Insight Generation
      ↓
Export Cleaned CSV
```

### ▶ Step 1 — Load the Data
- Pulled a student performance dataset from Kaggle
- Loaded into a Pandas DataFrame for inspection

### ▶ Step 2 — Pre-Cleaning Audit
Before touching anything, examined:
- Column names and what each represented
- Data types and memory structure
- Null values across every column

### ▶ Step 3 — Data Cleaning & Feature Engineering
- Created a working copy to preserve original data
- Renamed columns for clarity
- Replaced binary values (`1 = Yes`, `0 = No`)
- Filtered to students with `grade > 50` AND `attendance ≥ 75%`
- Engineered a new **Scholarship** column based on grade thresholds

### ▶ Step 4 — Visualizations & Insights

#### 📊 Finding 1 — Parental Education vs Student Grades
| Parent Education | Avg Student Grade |
|---|---|
| PhD Holder | 71 |
| Non-PhD | 64 |

A **7-point gap** — just from family background.

> ⚠️ But does a parent's PhD *cause* better grades? Almost certainly not.
> What the data is likely capturing is something deeper — study culture at home, access to resources, or an environment where academics are prioritized.
> **Correlation ≠ Causation.**

#### 📈 Finding 2 — Engagement vs Disengagement
| Student Type | Avg Grade |
|---|---|
| Academically active + part-time job | 77 |
| Low participation + no job | 71 |

Driven students tend to do more across the board — not less.

### ▶ Step 5 — Export
- Sorted the cleaned DataFrame
- Saved final output as `.csv`

---

## 💡 Key Takeaway

> Anyone can apply a function.
> The harder skill is questioning what your output is **actually telling you** — and what it **isn't**.

Data cleaning, transformation, visualization, and interpretation aren't separate steps. They're one continuous conversation with the data.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| `Python 3.10+` | Core language |
| `Pandas` | Data loading, cleaning, transformation |
| `NumPy` | Numerical operations |
| `Matplotlib` | Base visualizations |
| `Seaborn` | Statistical plots |
| `Kaggle` | Dataset source |

---

## 📁 Project Structure

```
student-performance-analysis/
│
├── data/
│   ├── raw/                  # Original Kaggle dataset
│   └── cleaned/              # Exported cleaned CSV
│
├── notebooks/
│   └── analysis.ipynb        # Main analysis notebook
│
├── visuals/
│   └── *.png                 # Generated charts
│
└── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/student-performance-analysis.git

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn

# 3. Open the notebook
jupyter notebook notebooks/analysis.ipynb
```

---

## 📬 Connect With Me

If this project resonates or you have feedback, let's connect on [LinkedIn](https://www.linkedin.com/in/prachi-ai1011/)!

---

*Still building. But now building with a critical eye. 🎯*

