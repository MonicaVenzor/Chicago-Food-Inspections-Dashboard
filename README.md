# 🍽️ Chicago Food Inspections – Data Analytics Project  

## 📌 Quick Summary  
This project explores **~297,000 food inspection records** from the City of Chicago.  
I worked through the **entire analytics process**: cleaning messy raw data, transforming it for analysis, and building an **interactive dashboard** to highlight key insights.  

- Cleaned and standardized the dataset using **Excel Power Query (M language)**  
- Created exploratory analysis with **PivotTables and PivotCharts**  
- Built a **Power BI dashboard** with filters, KPIs, and visuals for storytelling  

🔗 Dataset: [Chicago Food Inspections – data.gov](https://catalog.data.gov/dataset/food-inspections)  

---

## 🗂️ Dataset  
- **Source:** Public dataset from the Chicago Department of Public Health  
- **Size:** ~297,000 rows  
- **Key fields:**  
  - Inspection ID  
  - Business / Facility Type  
  - Inspection Date (Year, Month extracted)  
  - Results (Pass, Fail, Other)  
  - Risk (High, Medium, Low)  
  - Violations (codes & descriptions)  
  - Location (City, Address, Zip)  

---

## 🧹 Data Cleaning – Excel Power Query (M)  
The raw data had plenty of issues: typos, inconsistent categories, duplicates, and free-text violations.  

**Steps I took:**  
- Standardized city names (e.g., *Cchicago, Chciago → Chicago*)  
- Grouped facility types (e.g., *Bakery/Restaurant → Bakery*)  
- Simplified results into 3 buckets: **Pass, Fail, Other**  
- Expanded violations into rows, extracted valid codes (0–70)  
- Added time features (Year, Month) for trend analysis  
- Created flags (`Fail_Flag`, `Total_Flag`) to support KPI calculations  

---

## 📊 Data Modeling – Power BI  
- Added a **Date Table** for time intelligence  
- Built DAX measures:  
  - Total inspections  
  - Failed inspections  
  - Fail rate %  
  - Violations count  
  - % of fails in High Risk facilities  
- Connected **Food_Inspections** with the violations table for deeper analysis  

---

## 📈 Dashboard Highlights  
The dashboard was designed to be **clean, modern, and easy to interpret**.  

### KPIs  
- Total inspections  
- Failed inspections  
- Total violations  
- % of High Risk fails  

### Visuals  
- Pass vs Fail (donut)  
- Failures by Facility Type (bar)  
- Risk Level breakdown (donut)  
- Trend of inspections over time (line)  
- Chicago vs Suburbs + Top 10 Cities (bar)  
- Most common violations (bar & treemap)  

### Filters  
- Year  
- Facility Type  
- Risk Level  
- City  

---

## 🔑 Key Insights  
- **Restaurants** dominate both inspections and failures.  
- **High Risk facilities** drive ~74% of all failures.  
- Most inspections happen in **Chicago**, but suburbs like Evanston and Cicero also show relevant patterns.  
- **Sanitation and temperature control** are the most frequent violations.  
- Failures remain stable over time with minor seasonal variation.  

---

## 📂 Repository Structure  

Chicago-Food-Inspections-Dashboard/
│
├── Dataset/
│   └── README - Food_Inspections_pvt_sample.xlsx (Google Drive Link)
│
├── Dashboard/
│   ├── README - Food_Inspections_Dashboard.pbix           (Google Drive Link)
│   ├── Food_Inspections_Dashboard.pdf            Export estático
│   ├── Food_Inspections_Dashboard_Filter.pdf     Export estático with filters
│   └── ChicagoFoodInspectionsDashboardGif.gif    Demo gif
│
├── README.md                                   
└── SUMMARY.md                                  



---

## 🚀 How to View  
1. Open `Food_Inspections_pvt.xlsx` in Excel to see the cleaned dataset.  
2. Open `Food_Inspections_Dashboard.pbix` in Power BI for the interactive dashboard.  
3. Check `Food_Inspections_Dashboard.pdf` and `Food_Inspections_Dashboard_Filter.pdf` for a static version.
4. Watch `ChicagoFoodInspectionsDashboardGif.gif` for a quick preview.  

---

## 🛠 Tools & Skills Used  
- **Excel Power Query (M):** Data cleaning & transformation  
- **Power BI (DAX, Modeling, Visualization):** Dashboard building  
- **PivotTables & PivotCharts:** Exploratory analysis  
- **Data Storytelling:** Turning raw inspections into insights  

---

## 👩‍💻 About Me  
I’m building my **Data Analyst portfolio** with real-world datasets to showcase:  
- Strong data cleaning and transformation skills  
- Ability to design dashboards with clear insights  
- Focus on communicating findings in a simple, professional way  

📧 Email: venzorcame@gmail.com  
💼 LinkedIn: www.linkedin.com/in/monicavenzor
💻 GitHub: https://github.com/MonicaVenzor

---

👉 This project reflects the **full data analytics workflow**:  
messy raw data → cleaned & structured dataset → analytical model → clear dashboard with insights.  

