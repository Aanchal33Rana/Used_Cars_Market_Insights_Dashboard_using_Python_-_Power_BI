# Used Cars Price Analysis & Dashboard (Python & Power BI)

## Project Overview
This project analyzes a dataset of used cars (~4,000 rows) to uncover pricing trends, mileage patterns, and car age effects on resale value.  
It includes data cleaning, feature engineering, exploratory data analysis (EDA), and creating an interactive Power BI dashboard to visualize insights.

---

## Dataset
- **Source**: Kaggle - Used Car Price Prediction Dataset  
- **CSV file used**: `used_cars_cleaned.csv`  
- **Columns**:
  - `brand`, `model`, `model_year`, `milage`, `fuel_type`, `engine`, `transmission`, `ext_col`, `int_col`, `accident`, `clean_title`, `price`  
  - Engineered features: `Car_Age`, `Mileage_per_Year`

---

## Tools & Technologies Used
- **Python**: pandas, numpy, matplotlib, seaborn (data cleaning, feature engineering, and EDA)  
- **Power BI Desktop**: interactive dashboards and data visualization  
- **GitHub**: version control and portfolio hosting  

---

## Steps Performed

### 1. Data Cleaning & Preprocessing
- Removed duplicates and handled missing values  
- Converted `milage` and `price` to numeric types  
- Removed outliers for realistic analysis  

### 2. Feature Engineering
- `Car_Age` = Current Year - `model_year`  
- `Mileage_per_Year` = `milage` / `Car_Age`  

### 3. Exploratory Data Analysis (EDA)
- Scatter plots: Price vs Car Age, Price vs Mileage per Year  
- Bar charts: Average Price per Brand, Fuel Type Distribution  
- Summary metrics: Average Price, Total Cars, Average Mileage per Year  

### 4. Power BI Dashboard
- Key Metrics Cards: average price, total cars, average mileage  
- Slicers: Brand, Fuel Type, and Car Age  
- Visuals: scatter plots, bar charts, column charts  

---

## Key Insights
- Older cars generally have lower resale prices  
- Luxury brands maintain higher prices even with higher mileage  
- Cars with higher annual mileage tend to have lower prices  
- Most cars in the dataset are gasoline-powered  

---

## Deliverables
- `used_cars_cleaned.csv` (cleaned dataset)  
- Python scripts for data cleaning, feature engineering, and EDA  
- Power BI dashboard file (`.pbix`)  
- Summary tables (`brand_summary.csv`, `age_summary.csv`) for faster Power BI import  

---

## How to Run
1. Load `used_cars_cleaned.csv` in Python for further analysis or feature modifications.  
2. Open Power BI Desktop, import `used_cars_cleaned.csv`, and recreate the dashboard using the recommended layout.  
3. Use slicers to filter by Brand, Fuel Type, or Car Age to explore trends interactively.  
