# ✈️ Aviation Safety Analysis

## 📌 Project Objective

The goal of this project is to help a company identify the **safest and most reliable aircraft to purchase**, based on historical accident and incident data. This data-driven analysis provides actionable insights to support purchasing decisions in aviation operations.

---

## 🗂 Dataset

- **Source**: [FAA/NTSB Aviation Accident Data]
- **Rows**: 88889
- **Columns**: 30
- **Key fields used**:
  - `Make`, `Model`
  - `Engine.Type`, `Number.of.Engines`
  - `Amateur.Built`
  - `Total.Fatal.Injuries`, `Total.Serious.Injuries`
  - `Event.Date`, `Weather.Condition`
  - `Country`, `Location`

---

## ❓ Business Questions

The company seeks to answer:

1. **Which aircraft models have the lowest number of reported accidents?**
2. **If an accident occurs, which aircraft models tend to have the lowest injury and fatality rates?**
3. **What is the accident rate per aircraft model, considering how often each model appears?**
4. **For aircraft that are frequently involved in accidents, what types of engines do they use?**

---

## 🔬 Data Analysis workflow

This project involved the following steps:

- ✅ **Data Exploration**
  - Checked for missing values, data types, and distributions
- ✅ **Data Cleaning**
  - Handled missing values, converted dates, standardized column names
- ✅ **Univariate Analysis**
  - Accident counts by aircraft make/model
  - Amateur-built vs. professionally built aircraft
- ✅ **Bivariate Analysis**
  - Engine types vs. accident frequency
- ✅ **Multivariate Analysis**
  - Accident severity, engine type, and model combinations

---

## 📊 Key Findings

- Aircraft like **[Cessna 172, Cirrus SR22, etc.]** are among the most accident-reported models — though this reflects popularity as well.
- Some models showed **high accident frequency** but **low injury/fatality rates**, indicating good survivability.
- **Reciprocating engines** were the most common among accident-prone aircraft — typical of general aviation.
- **Amateur-built aircraft** had a non-trivial share of accidents; buyers should be cautious depending on mission use.

---

## 🛠 Tools Used

- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **Jupyter Notebook**
- Git for version control

---

## 📌 Recommendations

- ✅ Avoid aircraft with **low injury/fatality averages**,.
- ⚠️ Be cautious of models with high accident rates — even if popular.
- ✅ Some amatuer built aircraft have low crash risk-built where safety is paramount.
- ✅ Consider aircraft with **non-reciprocating engines** (e.g., turboprop, turbojet) for commercial operations.

---


## 📁 Folder Structure

```bash
.
├── README.md
├── archive.zip
├── Data/
│   ├── AviationData.csv
│   └── USState_Codes.csv
├── Notebooks/
│   ├── Accidents.ipynb
│   ├── cleaned_data.csv
│   └── United_States_data.csv

