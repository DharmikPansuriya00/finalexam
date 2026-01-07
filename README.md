# 📊 Student Performance Dashboard – Academic & Behavioral Insights

An interactive **Power BI** dashboard that analyzes students’ academic performance, attendance, and behavior across different grades, subjects, and terms. Designed as an exam-style end‑to‑end BI project to demonstrate real‑world data modeling, DAX, and storytelling skills.

> Total Duration: 2.5–3 hours  
> Total Marks: 50

---

## 🧾 Evaluation Criteria

| Component                         | Marks |
|-----------------------------------|-------|
| Data Modeling & Cleaning          | 10    |
| DAX Calculations                  | 10    |
| Visualizations & Storytelling     | 15    |
| Slicers, Filters & Drillthrough   | 10    |
| Optional Features                 | 5     |
| **Total**                         | **50** |

---

## 📂 Dataset

The project uses four related CSV files:

1. `Students.csv` – StudentID, Name, Gender, Class, Section  
2. `Scores.csv` – StudentID, Subject, ExamType, Score, MaxScore, Term  
3. `Attendance.csv` – StudentID, Date, Status (Present/Absent), Reason  
4. `Behavior.csv` – StudentID, Date, BehaviorType, Notes  

These files are modeled in a star‑schema–like structure with `Students` as the central dimension table.

---

## 🏗️ Data Modeling & Cleaning

Key modeling steps:

- Established relationships between Students, Scores, Attendance, and Behavior using `StudentID`.
- Cleaned missing or inconsistent values (e.g., attendance status, behavior notes, score outliers).
- Created calculated columns for:
  - Percentage Score per exam.
  - Term/Year extraction from date fields.
- Ensured proper data types (Date, Text, Whole Number, Decimal) for accurate aggregations.

---

## 🧮 DAX Measures

Core DAX measures implemented:

- **Total Students** – distinct count of students.
- **Average Score** – average percentage across subjects/terms.
- **Average Attendance %** – ratio of Present vs total days.
- **Exam-wise KPIs** – max, min, and average score by ExamType.
- **Behavior Metrics** – count of incidents by BehaviorType and severity (if applicable).

These measures power the visuals and enable drilldowns by Class, Section, Subject, and Term.

---

## 📈 Visualizations

The main report page includes:

- **Bar Chart** – Average scores by Subject and Class.  
- **Line Chart** – Performance trend across Terms or Exam Types.  
- **Donut Chart** – Distribution of Behavior Types.  
- **Table** – Student-wise scores with conditional formatting (e.g., green for ≥80%, red for <40%).  
- **Card Visuals** – KPIs such as:
  - Total Students  
  - Average Score  
  - Average Attendance  
  - Total Behavior Incidents  

You can also add your own screenshots here, for example:

```markdown


