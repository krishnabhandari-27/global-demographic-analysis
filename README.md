# 🌍 Global Demographic & Geographic Pattern Analysis

## 📌 Project Overview

This project analyzes global demographic and geographic patterns using live data from the REST Countries API. The objective is to explore how population is distributed across regions, examine the relationship between land area and population, analyze population density patterns, and compare independent vs non-independent territories.

The project demonstrates API data collection, data cleaning, feature engineering, exploratory data analysis (EDA), and insight generation.

---

## 📊 Dataset Source

Data was collected using:

https://restcountries.com/v3.1/all

### Selected Fields:
- name
- population
- area
- region
- subregion
- capital
- independent

Total countries analyzed: 250

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Requests

---

## 🧹 Data Preparation

Steps performed:

- Fetched live data from REST Countries API
- Flattened nested JSON structure
- Handled missing values
- Removed invalid entries (area = 0)
- Created new feature:

Population Density = Population / Area

- Checked duplicates and validated data types

---

## 🔎 Exploratory Data Analysis

### 1️⃣ Regional Population Share
- Calculated total population per region
- Computed percentage contribution
- Found that Asia contributes approximately 60% of global population

### 2️⃣ Area vs Population Relationship
- Computed correlation coefficient (~0.40)
- Used scatter plot and log-log transformation
- Found moderate positive relationship
- Concluded that land area alone does not strongly determine population size

### 3️⃣ Population Density Analysis
- Identified most densely populated countries
- Observed heavily right-skewed distribution
- Found that smaller territories tend to exhibit extremely high density

### 4️⃣ Independence-Based Comparison
- Compared independent vs non-independent territories
- Found non-independent regions have higher median population density
- Likely due to smaller land area and urban concentration

---

## 📈 Key Insights

- Global population is highly concentrated in Asia (~60%).
- Area and population show a moderate positive correlation.
- Population density is heavily skewed, with extreme outliers.
- Non-independent territories tend to be more densely populated.
- Large land area does not necessarily imply high population density.

---

## ⚠️ Limitations

- Snapshot dataset (no time-series analysis)
- No GDP or economic indicators included
- No migration or urbanization metrics
- Density affected by extreme outliers

---

## 🚀 Future Improvements

- Merge with World Bank GDP dataset
- Perform clustering analysis on countries
- Build interactive dashboard using Streamlit
- Add machine learning-based classification

---

## ▶️ How to Run

1. Clone the repository
2. Install requirements:

pip install -r requirements.txt

3. Run the notebook inside /notebooks

---

## 📌 Project Structure

global-country-analysis/
│
├── data/
│   └── countries_cleaned.csv
│
├── notebooks/
│   └── eda_analysis.ipynb
│
├── images/
│
├── README.md
│
└── requirements.txt

---

## 👨‍💻 Author

Krishna Bhandari  
BCA Student | Aspiring Data Scientist
