# 🏥 Health Activity Analytics Dashboard — Power BI

A one-page interactive Power BI dashboard built on 1,000 patient health records, answering 6 business questions across lifestyle, risk factors, and health segmentation.

![Dashboard Preview](dashboard_preview.png)

---

## 📌 Business Questions Answered

| # | Question | Visual Used |
|---|----------|-------------|
| 1 | Are users maintaining a balanced lifestyle (Steps, Sleep, Calories)? | KPI Cards + Gauge Chart |
| 2 | What lifestyle patterns indicate heart disease risk? | Heart Risk Bar + HD Rate by Smoker |
| 3 | Is there a relationship between Sleep and Physical Activity? | Scatter Plot with Trendline |
| 4 | How does BMI vary across Age Groups and Genders? | Clustered Bar Chart |
| 5 | What is the impact of smoking and alcohol on heart rate and BP? | Risk Factor Impact Combo Chart |
| 6 | Segment people based on health activity to suggest lifestyle changes | User Segmentation Donut |

---

## 🔍 Key Findings

- **Steps vs Sleep (r ≈ 0.007):** Daily steps average 10.72K — above the 10K target — but show virtually zero correlation with sleep quality. Physical activity alone does not drive better sleep in this cohort.

- **Alcohol & Blood Pressure:** Moderate alcohol consumption (4–6 units/week) correlates with the highest average systolic BP (114.4 mmHg), slightly higher than heavy drinkers (114.0) — suggesting a non-linear risk curve.

- **Counterintuitive Heart Disease Finding:** Overall heart disease prevalence is 9.3%. Non-smokers (9.6%) show marginally higher rates than smokers (7.9%), indicating that BMI and diabetes are stronger predictors of heart disease risk in this dataset than smoking status alone.

---

## 📊 Dashboard Visuals

| Visual | Description |
|--------|-------------|
| KPI Cards | Avg BMI (26.73), Heart Disease Rate (9.30%), Avg Steps (10.72K), Avg Sleep (6.91 hrs) |
| Gauge Chart | Avg Steps vs 10K target — users are exceeding the benchmark |
| Heart Risk Bar | Avg systolic BP by smoker status (Yes: 114.52 / No: 113.81) |
| Scatter Plot | Sleep hours vs Daily Steps by gender — flat trendline confirms no correlation |
| BMI by Age & Gender | Senior males have highest BMI (27.0); Young females lowest (25.8) |
| Risk Factor Impact | Combo chart: Avg BP + Avg Heart Rate across alcohol consumption levels |
| Heart Disease by Smoker | HD % — Non-smokers: 9.6% vs Smokers: 7.9% |
| User Segmentation | 48% Moderate, 32.4% Active, 13.2% High Risk, 6.4% Sedentary |

---

## 🛠️ Tools & Techniques

- **Tool:** Microsoft Power BI Desktop
- **Data:** Synthetic health dataset — 1,000 records, 16 columns
- **DAX Measures:** Avg BP, Avg Heart Rate, HD %, HD % by Smoker, Alcohol_Sort (custom sort column)
- **Power Query:** Split Blood_Pressure text column into Systolic/Diastolic numeric fields
- **Features Used:** Calculated columns, custom sort order, combo charts (dual Y-axis), gauge visual, donut segmentation, scatter trendline

---

## 📁 Dataset Columns

| Column | Type | Description |
|--------|------|-------------|
| Age, Gender | Demographic | Patient profile |
| BMI, Height_cm, Weight_kg | Physical | Body metrics |
| Daily_Steps, Exercise_Hours_per_Week | Activity | Physical activity levels |
| Hours_of_Sleep, Calories_Intake | Lifestyle | Daily habits |
| Heart_Rate, Blood_Pressure | Vitals | Cardiovascular markers |
| Smoker, Alcohol_Consumption_per_Week | Risk factors | Lifestyle risk indicators |
| Diabetic, Heart_Disease | Health outcomes | Binary outcome flags |

---

## 🚀 How to Open

1. Download `Health_Dashboard.pbix` from this repository
2. Open with **Power BI Desktop** (free download from Microsoft)
3. All data is embedded — no external connections needed
4. Use the **Gender/Age Group slicer** (top dropdown) to filter all visuals simultaneously

---

## 👤 Author

**Bhavya** — Data Analyst  
📍 New Delhi, India  
🔗 [LinkedIn](https://linkedin.com/in/) | [GitHub](https://github.com/)  
📚 Data Analytics with Generative AI — PW Skills (2025)  
🏦 Domain Experience: Banking (Indian Overseas Bank — RBI compliance, NPA analysis, KYC, fraud detection)
