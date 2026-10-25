# Campus-Placement-Analytics-Dashboard

### *Turning five years of campus recruitment data into decisions that improve placement outcomes.*

**Alternative taglines (pick one):**
- *From placement data to placement strategy.*
- *An end-to-end Power BI analytics solution for tracking, understanding and improving campus placements.*
- *Where hiring data meets actionable insight.*

---

## 📌 Project Overview

The **Campus Placement Analytics Dashboard** is a 5-page, interactive **Power BI** report built on a **MySQL** database. It analyses campus placement data for graduation years **2021-2025** across 16+ departments (BTech, BCA, BBA, MBA, B.Com, B.Sc.).

The dashboard helps placement cells, department heads and management answer questions such as:

- How many students are getting placed, and how does that compare to targets?
- Which departments, companies and package brackets drive placement results?
- At which recruitment round do most students drop off?
- Do CGPA, skills, internships, certifications and projects really affect packages?
- What concrete actions can improve placement outcomes next year?

> **Note:** This is a data analytics and BI project (dashboard + database), not a website.

---

## 🎯 Purpose & Objectives

- Track placement performance against **placement-rate, placed-student and salary targets**.
- Analyse **hiring patterns and selection-round drop-off** across companies.
- Identify the **gap between student skill supply and industry skill demand**.
- Measure the impact of **internships, certifications and projects** on packages.
- Provide **data-backed improvement strategies** for the placement cell.

---

## 🛠️ Tech Stack

| Layer | Tools / Technologies |
|---|---|
| **Data Storage** | MySQL (student, academic, company, application, internship and placement data) |
| **Data Collection / Import** | Excel / CSV |
| **Data Cleaning & Transformation** | Power Query |
| **Data Modelling & Calculations** | DAX (measures, KPIs, ratios, targets) |
| **Visualization & Reporting** | Microsoft Power BI Desktop |
| **Version Control** | Git & GitHub |

---

## 📊 Dashboard Pages & Features

The report has 5 pages with a shared navigation bar. Slicers for **Graduation Year**, **Department** and other fields filter all visuals on a page.

### 1️⃣ Executive Summary
A high-level snapshot of placement performance.
- **KPI cards:** Placement Rate vs Target, Placed Students vs Target, Average Package vs Salary Target (gauge), Total Companies Participated, Max Package.
- **Placement Rate by Department** (pie chart)
- **Placed vs Total Students** by graduation year (clustered column chart)
- **Placed Students by Offer Type**: Campus Placement vs PPO (donut)
- **Total Offers by Package Bracket**: <5, 5-10, 10+ LPA (donut)

### 2️⃣ Hiring & Selection Analytics
Company hiring patterns and student selection at each round.
- **Package (LPA) vs CGPA** scatter plot, colour-coded by department
- **Drop-off after every level:** Applied → Resume → Aptitude → GD → Technical → Final Offers
- **Average Package Offered by Company** (bar chart)
- **Average Interview Score by Round Type** (HR, Technical, Aptitude, GD)
- **Top Hiring Companies by Final Offers** (table with total)
- Slicers: Fields, Graduation Year, Department

### 3️⃣ Skills & Internship Impact
Employability, skill gaps and placement readiness.
- **Skill Demand Count** (bar chart)
- **Student Skill Supply vs Skill Demand** (table)
- **Placed Interns by Performance Rating** (Excellent / Good / Average / Poor)
- **Placed Students by CGPA Band**
- Slicers: Skill Category, Graduation Year, Department, Internship Duration (8-24 weeks)

### 4️⃣ Certifications, Projects & Recruitment Criteria
How credentials and eligibility rules shape outcomes.
- **KPI cards:** Total Certified Students, Average Projects per Student, Total Applications, Average Package
- **Company Eligibility & Round Cutoffs** (package, min CGPA, max backlogs, aptitude cutoff)
- **Project Domain Impact on Salary Package** (scatter)
- **Recruitment Stage Conversion & Drop-off** (funnel)
- **Top Certifications by Student Share & Average Package** (treemap)
- Slicers: Department, Company Sector, Offer Type

### 5️⃣ Actionable Improvement Plans & Action Strategies
Four data-driven recommendations:
1. **Interview Technical Conversion:** mandatory 4-week coding bootcamps and mock technical panels before drive season.
2. **High-Value Certification Support:** subsidised vouchers (AWS, MySQL, Microsoft) for domains with lower average packages.
3. **Academic Eligibility Remediation:** early tutoring for students with 1-2 backlogs or CGPA near cutoffs (about 6.0-6.5).
4. **Corporate Relations & Tier-1 Outreach:** target product and high-paying sectors to grow the 10+ LPA share.

---

## ✨ Key Highlights

- ✅ Database-connected report (MySQL → Power Query → Power BI)
- ✅ 5 years of data (2021-2025) across 16+ departments and 31 companies
- ✅ Target vs actual KPI tracking with DAX measures
- ✅ Full recruitment funnel analysis, from application to final offer
- ✅ Skill supply vs demand gap analysis
- ✅ Interactive slicers and consistent navigation across pages
- ✅ Ends with actionable recommendations, not just charts

---

## 💡 Business Insights

### Placement performance
- **577 students were placed** over 5 years (about 109-124 per year) out of roughly 1,000 total, an overall placement rate of about **57-58%**.
- The latest-year KPI shows a **55.34% placement rate (114 placed)**, which is **below the 85% target** (-34.89%) and **43% short of the 200-student goal**.
- The **average package is 8.52 LPA**, slightly above the 8.00 LPA target, and the **highest package is 23.48 LPA**.
- The student pool grew from about 183 (2021) to about 206 (2025), but placements stayed flat at about 110-125. **Placement growth is not keeping pace with batch size.**

### Departments and offers
- **BTech Computer Science (~69%), Civil Engineering (~67%) and Data Science (~66%)** lead on placement rate. The lowest department is around 40%.
- **74% of placements come from campus drives and 26% from PPOs**, so internships are already a meaningful pipeline.
- **60% of offers fall in the 5-10 LPA bracket**, 27% are 10+ LPA and about 13% are below 5 LPA.

### Hiring and selection
- **Recruitment funnel (~3,000 applications):** about 2,150 clear resume screening, about 1,680 aptitude, about 1,230 GD, about 850 technical, and **~790 final offers**. The **steepest drops are at the aptitude/GD and technical stages**.
- **Mass recruiters give volume; product companies give high packages.** Accenture, Capgemini, Byju's and Bajaj Finserv account for most offers. Microsoft, Amazon, Adobe, Samsung R&D and Google average **21-27 LPA** but make very few offers (Adobe and Amazon have only 2 each).
- **CGPA alone does not predict package.** The scatter plot shows high packages (30+ LPA) at a wide range of CGPAs, so skills and interview performance matter more than marks.
- **Average interview scores are similar across rounds (~56-59)**, which suggests no single round is far weaker than the others.

### Skills, internships and certifications
- **Student skill supply is much larger than demand for many skills** (e.g. Angular: 77 students vs 2 openings; AWS: 90 vs 7), while **Communication, MATLAB, AutoCAD, CI/CD and REST API Design** are in highest demand. Students are skilling broadly, not in line with what recruiters ask for.
- **Strong internship performers get placed:** about 65% of placed interns were rated *Good* or *Excellent*, and only about 8% *Poor*.
- **Most placed students sit in the 6.0-7.9 CGPA range**, so placement success is not limited to top scorers.
- **AI/ML projects are linked to the highest average package (~9.7 LPA)**, ahead of Business, Web Development, Core Engineering and Data Science projects.
- With **541 certified students** but only **1.07 projects per student**, hands-on project work is a clear area for growth.
- Company eligibility criteria (CGPA cutoffs about 5-7, backlog limits of 1-2) make **academic remediation** a direct way to widen opportunities.

---

## 🖼️ Screenshots

| Page | Preview |
|---|---|
| Executive Summary | ![Executive Summary](https://github.com/Tavleenkaur17/Campus-Placement-Analytics-Dashboard/blob/main/Executive%20Summary.png) |
| Hiring & Selection Analytics | ![Hiring and Selection](https://github.com/Tavleenkaur17/Campus-Placement-Analytics-Dashboard/blob/main/Hiring%20And%20Selection%20Analytics.png) |
| Skills & Internship Impact | ![Skills and Internship](https://github.com/Tavleenkaur17/Campus-Placement-Analytics-Dashboard/blob/main/Skills%20and%20Internship%20Impact.png) |
| Certifications, Projects & Recruitment Criteria | ![Certifications](https://github.com/Tavleenkaur17/Campus-Placement-Analytics-Dashboard/blob/main/Certifications%2C%20Projects%20and%20Recruitment%20Criteria%20Analytics.png) |
| Actionable Improvement Plans | ![Action Plans](https://github.com/Tavleenkaur17/Campus-Placement-Analytics-Dashboard/blob/main/Actionable%20Improvement%20Plans%20and%20Action%20Strategies.png) |


## 🚀 Future Scope

- Automatic scheduled refresh and publishing to Power BI Service
- Predictive models for placement probability from CGPA, skills and internships
- Row-level security for department-wise access
- A web portal embedding the dashboard

---

## 👩‍💻 Author

Tavleen Kaur | BCA-3C (5th semester) 

⭐ If you found this project useful, please star the repository!
