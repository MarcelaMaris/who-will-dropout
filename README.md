<p align="center">
  <img src="docs/cover.png" width="100%" alt="Student Dropout Analytics Dashboard cover">
</p>

## <img src="icons/education.png" width="50">  &nbsp;&nbsp;Who Will Drop Out? — Student Engagement & Retention Analytics
<br>

![Python](https://img.shields.io/badge/Python-3.10%2B-0A3756?style=flat&logo=python&logoColor=F5F7FA&labelColor=E8AA3A)
![Pandas](https://img.shields.io/badge/Pandas-lib-0A3756?style=flat&logo=pandas&logoColor=F5F7FA&labelColor=E8AA3A)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-0A3756?style=flat&logo=jupyter&logoColor=F5F7FA&labelColor=E8AA3A)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-0A3756?style=flat&logo=powerbi&logoColor=F5F7FA&labelColor=E8AA3A)
![Cohorts](https://img.shields.io/badge/Analysis-Cohorts-0A3756?style=flat&logo=academia&logoColor=F5F7FA&labelColor=E8AA3A)

> This project analyses **student engagement, retention, and dropout behaviour** in online education using the  
> **Open University Learning Analytics Dataset (OULAD)**.
>
> The objective is to understand **when students disengage**, **which behavioural patterns are associated with dropout**,  
> and **how early warning signals can be operationalised** through analytics and dashboards.
>
> The project combines **Python-based analysis** with a **Power BI executive dashboard**, translating behavioural data  
> into actionable insights for tutors, course designers, and academic managers.
> 
> It is designed to mirror how a data analyst or business analyst would investigate retention problems in a real educational platform.

---

## <img src="icons/objectives.png" width="30">  &nbsp;&nbsp;Objectives

- Analyse **dropout and retention patterns** in large-scale online learning.
- Identify **early disengagement signals** using behavioural and temporal features.
- Segment students into **engagement profiles** based on VLE interaction patterns.
- Explore how **engagement consistency vs. intensity** affects academic outcomes.
- Translate analytical findings into **monitoring tools and retention insights**.

---

## <img src="icons/features.png" width="30">  &nbsp;&nbsp;Key Analyses & Features

- **Exploratory Data Analysis (EDA):**  
  Demographic, academic, and socioeconomic patterns related to student outcomes.

- **Engagement Feature Engineering:**  
  Click volume, active days, early vs. late engagement, inactivity gaps.

- **Correlation & Feature Screening:**  
  Numeric correlation analysis and baseline feature importance to identify relevant behavioural signals.


- **Engagement Funnel:**  
  Tracking progression from *Registered → Active → Consistent → Completed* to identify critical drop-off points.

- **Cohort Retention Analysis:**  
  Heatmap-based visualisation of retention by module presentation and course progress.

- **Behavioural Segmentation:**  
  K-means clustering to identify low, moderate, and high engagement profiles.

- **Outcome Mapping:**  
  Linking engagement clusters to withdrawal, failure, pass, and distinction rates to support targeted intervention strategies.
---

## <img src="icons/dataset.png" width="30">  &nbsp;&nbsp;Dataset

**Source:**  
Open University Learning Analytics Dataset (OULAD)  
[https://analyse.kmi.open.ac.uk/open_dataset](https://analyse.kmi.open.ac.uk/open-dataset)

**Key Tables Used**
- `studentInfo.csv` — demographics and final results  
- `studentRegistration.csv` — registration and withdrawal timing  
- `courses.csv` — module metadata  
- `studentVle.csv` — VLE interaction logs  
- `studentAssessment.csv` — assessment submissions and scores  

⚠️ **Data availability note**  
Raw OULAD files are **not included** in this repository due to size and licensing constraints.

To run the notebook end-to-end:
1. Download the dataset from the official OULAD website.
2. Place the CSV files inside `data/raw/`.

If raw data are missing, the notebook raises a clear `FileNotFoundError` explaining how to obtain them.

---

## <img src="icons/dashboard.png" width="30">  &nbsp;&nbsp;Interactive Dashboard


The analytical results are summarised in a **single-page Power BI dashboard**, designed for non-technical stakeholders.

### Dashboard structure
1. **How many students stay vs. leave?**  
   KPI cards showing total students, dropout rate, pass rate, distinction rate, and early disengagement.

2. **When do students disengage?**  
   - Engagement funnel highlighting major behavioural drop-offs.  
   - Cohort retention heatmap showing that most disengagement occurs in the first 10–20% of the module.

3. **Which behavioural profiles are at risk?**  
   Engagement clusters linked to academic outcomes, revealing that consistency — not intensity — drives success.

**Dashboard (PDF – static version):**  
[Download Dashboard (PDF)](docs/dashboard/Who_Will_Drop_Out_Dashboard.pdf)

**Power BI interactive file (.pbix):**  
Available in the [`PowerBI/`](PowerBI/) folder (requires Power BI Desktop).

---

## <img src="icons/conclusions.png" width="30">  &nbsp;&nbsp;Key Insights

- **Dropout is heavily front-loaded:**  
  Most disengagement happens within the first weeks of the module.

- **Consistency matters more than intensity:**  
  Moderately but consistently engaged students outperform highly active but irregular learners.

- **Behavioural profiles are highly predictive:**  
  Low-engagement students almost always withdraw, while moderately engaged learners show the strongest outcomes.

- **Early warning signals are behavioural:**  
  Inactivity gaps, early clicks, and last interaction timing are stronger indicators than demographics.

---

## <img src="icons/impact.png" width="30">  &nbsp;&nbsp;Business & Educational Impact

- Enables **early identification of at-risk students**.
- Supports **targeted, data-driven interventions**.
- Provides a scalable framework for **retention monitoring** in online education.
- Bridges analytics and decision-making through a **dashboard-ready output**.

---

## <img src="icons/techstack.png" width="30">  &nbsp;&nbsp;Tech Stack

- **Languages & Libraries:** Python (3.10), Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn (Random Forest, K-Means)  
- **Environment:** Jupyter Notebook  
- **BI & Visualisation:** Power BI  
- **Data Handling:** CSV-based workflow with Pathlib  
- **Version Control:** Git & GitHub  

---

This project was inspired by personal experience in online education and reflects a strong interest in using data to improve learning experiences and retention outcomes.

---
<p align="center">
  <sub>📊 Designed & developed by <b>Marcela Maris</b> — Data Analytics Portfolio</sub><br>
  <sub><i>Learning Analytics • Retention Modelling • Behavioural Insights</i></sub>
</p>
