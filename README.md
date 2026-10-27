📊 Laptop Price & Market Analytics
Python Pandas NumPy Plotly scikit-learn Streamlit Power BI License

An end-to-end Data Analytics & ML project — from raw data to an interactive Streamlit web app.

📊 Dashboard Preview • 🚀 Workflow • 📈 KPIs • 🧠 Insights • 🛠 Tech Stack • ▶️ How to Run

📋 Table of Contents
Overview
Dashboard Preview
Dataset Information
Project Workflow
Key Performance Indicators
Dashboard Visualizations
Business Insights
Technologies Used
Project Structure
How to Run
🔍 Overview
This project performs a comprehensive analysis of the laptop market using a dataset of 27,456 laptop records across 10 brands. It covers:

✅ Data Cleaning — handling missing values, duplicates, and type conversions
✅ Exploratory Data Analysis (EDA) — uncovering trends across brands, specs, and pricing
✅ Feature Engineering — deriving priority scores, usage categories, and CPU/GPU labels
✅ Interactive Visualizations — Plotly-powered charts for deep exploration
✅ Machine Learning — price prediction using Random Forest Regressor
✅ Streamlit Web App — live interactive dashboard with filters and ML price predictor
✅ Power BI Dashboard — business intelligence report with KPI cards
📊 Dashboard Preview
Laptop Market Analysis Dashboard

📂 Dataset Information
Property	Value
Dataset Name	Laptop Sales Dataset
Total Records	27,456
Total Features	18
File Format	CSV
Brands Covered	10 (ASUS, MSI, HP, Dell, Lenovo, ACER, Apple, CASPER, MONSTER, Huawei)
Key columns include: brand, name, price, cpu, gpu, storage, ram, os, usage_purpose, and engineered priority scores.

Note: ~38% of records have no dedicated GPU (these use integrated graphics and are filled accordingly during cleaning).

🚀 Project Workflow
Raw Laptop Dataset (CSV)
        │
        ▼
 Data Cleaning (Python)
  ├── Handle missing values
  ├── Remove 2,846 duplicates
  └── Standardize data types
        │
        ▼
 Exploratory Data Analysis
  ├── Brand distribution
  ├── Price distribution
  ├── OS market share
  └── Hardware trends (RAM, GPU, Storage)
        │
        ▼
 Feature Engineering
  ├── CPU brand extraction
  ├── Priority scoring (CPU, GPU, RAM, OS, Storage)
  └── Usage purpose classification (Gaming / Office / Daily)
        │
        ▼
 Advanced Visualizations (Plotly + Seaborn)
  ├── Interactive bar & scatter charts
  ├── Correlation heatmaps
  └── Price outlier boxplots
        │
        ▼
 Machine Learning — Price Prediction
  └── Random Forest Regressor
        │
        ▼
 Power BI Dashboard
  └── Business Insights Report
📈 Key Performance Indicators (KPIs)
KPI	Value
📦 Total Laptops	24,610 (after deduplication)
💰 Total Sales	₺2.27 Billion
📊 Average Price	₺92,220
🏷 Total Brands	10
🎮 GPU Models	36
📊 Dashboard Visualizations
Chart	Type	Insight
Operating System Share	Pie Chart	FreeDOS & Windows dominate
Average Price by RAM	Line Chart	Higher RAM → Higher average price
Sales by Usage Purpose	Bar Chart	Gaming/Design drives 72% of revenue
Laptop Count by Brand	Bar Chart	ACER, HP, ASUS are most listed
Top Brands by Sales	Horizontal Bar	MSI leads with ₺0.53bn
GPU Distribution	Donut Chart	Integrated GPU laptops form 37%
🧠 Business Insights
MSI generated the highest overall sales (₺0.53bn), despite not being the most-listed brand — indicating a premium pricing strategy.
Gaming & Design laptops contribute ~72% of total revenue, despite representing fewer listings than Office/Daily laptops.
Average laptop price increases with RAM capacity — 96GB RAM laptops average ₺200,000+.
FreeDOS and Linux account for ~37% of OS share, suggesting strong demand for the developer/budget segment.
RTX-series GPUs are the most common high-performance GPU options across brands.
ACER, HP, and ASUS have the widest product portfolio, but MSI and ACER lead in revenue per unit.
🛠 Technologies Used
Python Stack
Library	Purpose
pandas	Data manipulation and cleaning
numpy	Numerical computation
matplotlib	Static visualizations
seaborn	Statistical charts
plotly	Interactive visualizations
scikit-learn	Price prediction (Random Forest)
openpyxl	Excel export support
jupyter	Notebook environment
BI & Reporting
Tool	Purpose
Power BI Desktop	Interactive dashboard
DAX	Calculated measures and KPIs
Power Query	Data transformation
📁 Project Structure
Laptop-Price-Market-Analytics/
│
├── app.py                          ← Streamlit web app
├── Laptop_Sales_Analysis.ipynb     ← Main analysis notebook
├── Laptop-sale-analysis.csv        ← Raw dataset
├── Laptop_Cleaned_Dataset.csv      ← Cleaned dataset (post-processing)
├── Laptop Sales Dashboard.pbix     ← Power BI dashboard file
├── Images/
│   └── Laptop Sales Dashboard.jpg  ← Dashboard screenshot
├── README.md                       ← This file
├── requirements.txt                ← Python dependencies
├── REPORT.PDF                      ← Full project report
└── LICENSE                         ← MIT License
▶️ How to Run
🌐 Streamlit Web App (Recommended)
1. Install dependencies:

pip install -r requirements.txt
2. Launch the app:

streamlit run app.py
Opens automatically at http://localhost:8501 — features brand/OS/price filters, KPI cards, 10+ interactive charts, and the ML price predictor.

🐍 Python Notebook
jupyter notebook Laptop_Sales_Analysis.ipynb
Or open in VS Code with the Jupyter extension.

📊 Power BI Dashboard
Open Laptop Sales Dashboard.pbix using Power BI Desktop (free download from Microsoft).

📄 License
This project is licensed under the MIT License — see the LICENSE file for details.
