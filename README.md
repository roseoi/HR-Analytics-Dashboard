# HR Analytics Project
A portfolio project combining Python data analysis and Power BI dashboard development.

This project demonstrates an end-to-end HR analytics workflow, including data cleaning, feature engineering, employee attrition modelling, training ROI analysis, and dashboard reporting.

---

## Repository Structure

HR-Analytics-Project/
│
├── data/                               # Dataset(s)
├── notebooks/
│   └── HR_Data_Analysis.ipynb          # Jupyter Notebook (Python)
├── dashboard/
│   ├── HR_RB.pdf                       # Power BI Dashboard
│   └── HR_Data_JupyterNotebook.pdf     # Notebook PDF (Python output)
└── README.md


## Power BI Dashboard Summary

### 1. HR Dashboard Overview  
(See HR_RB.pdf, page 1)

- Total employees, new hires, exits  
- Gender distribution and age groups  
- Engagement, satisfaction, and work-life balance scoring  
- Headcount trend (2018–2023)  
- Department and diversity breakdowns  

### 2. Workforce Analysis  
(See HR_RB.pdf, page 2)

- Employee count by department  
- Pay zone structure  
- Demographic analysis  
- DepartmentType slicer and filtering  

### 3. Training and Development  
(See HR_RB.pdf, page 3)

- Internal vs external training investment  
- Training outcomes (completed, passed, failed, incomplete)  
- Programme-level training spending  
- Monthly spending trends  
- Training success rate (52.5%)

---

## Python Analysis Summary

### 1. Data Loading and Inspection  
(Notebook PDF pages 1–2)

- Loaded a 3000-row HR dataset  
- Inspected data structure and missing values  
- Converted date columns (StartDate, ExitDate, DOB, Survey Date, Training Date)

### 2. Feature Engineering  
(Notebook PDF page 3)

Created new analytical variables:

- TenureDays, TenureYears  
- Age  
- Attrition (binary flag)  
- TrainingCostPerDay  

### 3. Exploratory Data Analysis

- Attrition by BusinessUnit  
- Engagement vs Satisfaction  
- Age distribution by attrition (KDE curves)  
- Several visual insights produced using Seaborn and Matplotlib  

### 4. Attrition Prediction Model  
(Notebook PDF pages 5–6)

- Target: Attrition  
- Features included age, tenure, engagement score, satisfaction score, work-life balance, performance score, gender, business unit  
- Preprocessing using OneHotEncoding and StandardScaler  
- Model: RandomForestClassifier  
- Final accuracy: approximately 85%  
- Feature importance visualization generated

### 5. Survival Analysis  
(Notebook PDF pages 7–8)

- Kaplan–Meier survival curve for overall tenure  
- Department-level survival functions comparing retention  

### 6. Employee Clustering  
(Notebook PDF page 8)

- KMeans clustering (k=3) applied to Engagement, Satisfaction, and Work-Life Balance  
- Cluster labels added to dataset  

### 7. Training Analysis and ROI  
(Notebook PDF pages 9–12)

- Performance vs training outcomes (boxplots)  
- Training cost vs engagement and satisfaction  
- Custom ROI Index calculated:

ROI = (Performance + Satisfaction) - (Attrition * 100)

- ROI by training programme  
- Bar chart and annotated scatterplot to evaluate programme effectiveness  

---

## Skills Demonstrated

- Python: Pandas, Seaborn, Matplotlib, Scikit-Learn, Lifelines, Statsmodels  
- Feature engineering, EDA, machine learning, clustering, survival analysis  
- Training evaluation and ROI modelling  
- Power BI: data modelling, DAX, report design  
- HR analytics: attrition modelling, training insights, workforce analytics  

---
