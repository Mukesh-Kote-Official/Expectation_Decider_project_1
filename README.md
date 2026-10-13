# 🎯 Expectation Decider – Probability Analysis

[![Python](https://img.shields.io/badge/Python-Analysis-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)]()
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)


**Mathematics & Advanced Statistics | Project PR1**

A probability analysis of 200 students to understand which factors affect the chance of passing a competitive mathematics exam.

---

---

## 📁 Repository Structure

```
├── README.md                  # Project overview (this file)
├── Expectation_Decider.ipynb  # Practical work (code + markdown)
├── student_data.csv           # Dataset (200 students, AI-generated)
└── Expectation_Decider_Explnation.pdf   # Handwritten theory (photos converted to PDF)
```

---

## 📊 Dataset

AI-generated sample dataset of **200 students** (`student_data.csv`). The notebook loads this file directly, so results are the same every time you run it.

| Field | Description |
|---|---|
| `student_id` | Unique ID (1–200) |
| `study_hours` | Hours studied per week |
| `attendance` | Attendance percentage in lectures |
| `group_discussion` | Participation in group discussions (Yes/No) |
| `previous_test_score` | Marks out of 100 in last internal test |
| `final_exam_pass` | Result of competitive exam (Pass/Fail) |

---

## ✅ Tasks Covered

| # | Topic | What was done |
|---|---|---|
| 1 | Basics of Probability | Definition, terminology, 3 event examples from the data |
| 2 | Types of Events | Empirical P(Pass) = 124/200 = 0.62; Theoretical P(ID divisible by 5) = 40/200 = 0.20 |
| 3 | Random Variable & Distribution | X = passes among 3 students, Binomial(3, p) table, mean = 1.86, variance = 0.7068 |
| 4 | Venn Diagram | Study > 10 hrs vs Attendance > 80%, overlap = 56 students |
| 5 | Contingency Table | Joint = 0.395, Marginal P(Pass) = 0.62, Conditional P(Pass \| GD=Yes) = 0.6529 |
| 6 | Relationships | Intuition of conditional probability; independence check (formula + chi-square test) |
| 7 | Bayes' Theorem | P(Pass \| High attendance) = 7/9 ≈ 0.7778 |
| 8 | Final Summary | Pass rate by factor + correlations |


---

## 🧠 Key Findings

- **Overall pass rate: 62%.** Of 200 students, 124 passed and 76 failed (P(Pass) = 124/200 = 0.62). This is the baseline that every other factor is compared against.

- **Study hours is the strongest factor.** Students studying more than 10 hrs/week passed 69.7% of the time, versus 50.6% for the rest, a gap of 19.1 points. It also has the highest correlation with passing (0.23).

- **Attendance is almost as strong.** Students above 80% attendance passed 72.2% of the time, versus 53.6% for the rest, a gap of 18.6 points (correlation 0.21).

- **Previous test score and group discussion have a smaller effect.** Both add only about 8 points (66.0% vs 58.0% for score ≥ 60, and 65.3% vs 57.0% for group discussion).

- **Group discussion and passing are independent, not mutually exclusive.** P(Yes) × P(Pass) = 0.375 is close to the actual P(Yes and Pass) = 0.395, and the chi-square p-value is 0.30 (above 0.05), so the small gap is likely noise. They are not mutually exclusive because 79 students did both.

- **Bayes' theorem result: 77.8%.** Using the given history, P(Pass) works out to 2/3 (66.7%), and P(Pass | high attendance) = (0.70 × 0.667) / 0.60 = 0.778. Knowing a student has high attendance raises their pass chance by about 11 points.



---


---

## 🛠️ Tech Stack

Python • NumPy • Pandas • Matplotlib • SciPy • Jupyter Notebook

---

## 👨‍💻 Author

**Mukesh kote**
