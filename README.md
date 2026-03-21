# 👥 HR Analytics Dashboard — Employee Attrition Analysis

> An interactive HR Analytics Dashboard built with **Power BI**, analyzing employee attrition patterns across departments, age groups, education fields, gender, and job roles. Helps HR teams identify retention risks and make data-driven workforce decisions.

---

## 🖼️ Dashboard Preview

![HR Analytics Dashboard](HR%20Dashboard.pdf)

> 💡 *For best GitHub rendering, replace the PDF reference above with a `.png` screenshot of the dashboard.*

---

## 📌 Overview

This project dives into a corporate HR dataset to answer critical workforce questions:

- 🔴 **Who is leaving?** — Attrition by department, age, gender, and education
- 📊 **Why are they leaving?** — Satisfaction scores, overtime, work-life balance
- 🏢 **Which roles are at risk?** — Job satisfaction ratings by role
- 📅 **How long do employees stay?** — Tenure, promotion history, and managerial stability

---

## 🎯 Key KPIs (from Dashboard)

| Metric | Value |
|--------|-------|
| 👨‍💼 Overall Employees | **1,470** |
| 🚪 Total Attrition | **237** |
| 📉 Attrition Rate | **16.12%** |
| ✅ Active Employees | **1,233** |
| 🎂 Average Age | **37** |

---

## 📈 Key Visualizations

| Chart | Description |
|-------|-------------|
| 🥧 Pie Chart | Department-wise Attrition — R&D (56.12%), Sales (38.82%), HR (5.06%) |
| 📊 Bar Chart | Employee count by Age Group & Gender |
| 📋 Matrix Table | Job Satisfaction Rating (1–4) by Job Role |
| 📉 Bar Chart | Education Field wise Attrition |
| 🍩 Donut Charts | Attrition Rate by Gender across 5 Age Bands |

---

## 🗂️ Repository Structure

```
HR-Analytics-Dashboard/
│
├── HR Dashboard.pbix        # Power BI workbook (interactive)
├── HR Dashboard.pdf         # Exported static dashboard
├── HR Data.xlsx             # Raw dataset
└── README.md                # Project documentation
```

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|------|---------|
| [Microsoft Power BI](https://powerbi.microsoft.com/) | Dashboard design & visualization |
| Microsoft Excel (`.xlsx`) | Raw data source |
| DAX | Calculated columns & KPI measures |
| Power Query | Data transformation |

---

## 📦 Dataset

The dataset contains **HR records** for 1,470 employees with **40+ attributes** covering demographics, job details, satisfaction metrics, and attrition status.

### 🗃️ Column Reference

| Column | Type | Description |
|--------|------|-------------|
| `emp no` | ID | Staff ID (e.g. STAFF-1) |
| `Employee Number` | Numeric | System employee number |
| `Age` | Numeric | Employee age |
| `CF_age band` | Category | Age group — Under 25, 25–34, 35–44, 45–54, Over 55 |
| `Gender` | Category | Male / Female |
| `Marital Status` | Category | Single, Married, Divorced |
| `Over18` | Flag | All employees are over 18 (Y) |
| `Department` | Category | R&D, Sales, HR |
| `Job Role` | Category | Sales Executive, Research Scientist, Lab Technician, etc. |
| `Job Level` | Numeric | 1 (entry) to 5 (executive) |
| `Job Involvement` | Numeric | 1–4 scale |
| `Job Satisfaction` | Numeric | 1 (low) to 4 (high) |
| `Education` | Numeric | 1=High School → 5=Doctoral |
| `Education Field` | Category | Life Sciences, Medical, Marketing, Technical, Other |
| `Business Travel` | Category | Non-Travel, Travel Rarely, Travel Frequently |
| `Over Time` | Flag | Yes / No |
| `Attrition` | Flag | Yes (left) / No (stayed) |
| `CF_attrition label` | Category | Ex-Employees / Current Employees |
| `CF_current Employee` | Flag | 1 = Active, 0 = Left |
| `Monthly Income` | Numeric | Monthly salary (£) |
| `Daily Rate` | Numeric | Daily pay rate |
| `Hourly Rate` | Numeric | Hourly pay rate |
| `Monthly Rate` | Numeric | Monthly rate |
| `Percent Salary Hike` | Numeric | Last salary increase % |
| `Performance Rating` | Numeric | 1–4 performance score |
| `Environment Satisfaction` | Numeric | 1–4 scale |
| `Relationship Satisfaction` | Numeric | 1–4 scale |
| `Work Life Balance` | Numeric | 1–4 scale |
| `Stock Option Level` | Numeric | 0–3 |
| `Distance From Home` | Numeric | Distance to office (km) |
| `Total Working Years` | Numeric | Career experience in years |
| `Years At Company` | Numeric | Tenure at current company |
| `Years In Current Role` | Numeric | Years in current job role |
| `Years Since Last Promotion` | Numeric | Recency of last promotion |
| `Years With Curr Manager` | Numeric | Stability of reporting relationship |
| `Num Companies Worked` | Numeric | Previous employers count |
| `Training Times Last Year` | Numeric | Training sessions attended |
| `Standard Hours` | Numeric | Fixed at 80 for all employees |
| `Employee Count` | Numeric | Fixed at 1 per row |

### 🔢 Sample Records

| Staff ID | Age | Gender | Department | Job Role | Attrition | Monthly Income | Over Time | Work Life Balance |
|----------|-----|--------|------------|----------|-----------|---------------|-----------|-------------------|
| STAFF-1 | 41 | Female | Sales | Sales Executive | ✅ Yes | £5,993 | Yes | 1 |
| STAFF-2 | 49 | Male | R&D | Research Scientist | ❌ No | £5,130 | No | 3 |
| STAFF-4 | 37 | Male | R&D | Lab Technician | ✅ Yes | £2,090 | Yes | 3 |
| STAFF-5 | 33 | Female | R&D | Research Scientist | ❌ No | £2,909 | Yes | 3 |
| STAFF-7 | 27 | Male | R&D | Lab Technician | ❌ No | £3,468 | No | 3 |

---

## 💡 Key Insights

- 🔴 **R&D has the highest attrition** at 56.12%, despite being the largest department
- 👶 **Age group 25–34** sees the sharpest attrition — 112 employees left
- ⏱️ **Overtime is a strong attrition signal** — many departing employees had `Over Time = Yes`
- 🎓 **Life Sciences & Medical** graduates account for the most attritions by education field
- 👩 **Gender gap in younger cohorts** — females under 25 show higher relative attrition (52%)
- 💼 **Sales Executives** have the highest Job Satisfaction survey count (326), suggesting scale, not necessarily satisfaction
- 📉 **Low-income roles** (Lab Technicians at ~£2,000–£3,500/mo) show higher attrition than management roles

---

## 🔧 Future Improvements

- [ ] Add DAX measures documentation
- [ ] Build a drill-through page per department
- [ ] Add a predictive attrition model using Python / ML
- [ ] Publish to Power BI Service for live sharing
- [ ] Add a data cleaning / preprocessing notebook

---

## 🚀 How to Use

1. **View Dashboard** — Open `HR Dashboard.pdf` for the static export
2. **Explore Interactively** — Open `HR Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. **Access Raw Data** — Open `HR Data.xlsx` in Excel or load it into Power BI / Python

---

## 🙋 Author

**Mindbender66**
- 🐙 GitHub: [@Mindbender66](https://github.com/Mindbender66)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
