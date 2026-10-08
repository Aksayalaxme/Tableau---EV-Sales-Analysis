# 🚗 Electric Vehicle Sales Analysis – Tableau

## 📌 Project Overview

This project is an interactive **Electric Vehicle (EV) Sales & Population Analysis Dashboard** developed using **Tableau**.

The dashboard analyzes electric vehicle data to understand EV adoption patterns across different **vehicle types, manufacturers, models, model years, states, electric ranges, and CAFV eligibility categories**.

The objective is to transform raw electric vehicle data into an interactive visual dashboard that can help users identify trends, compare manufacturers and models, and understand the geographical distribution of electric vehicles.

---

## 🎯 Project Objectives

* Analyze the overall electric vehicle population.
* Compare **Battery Electric Vehicles (BEVs)** and **Plug-in Hybrid Electric Vehicles (PHEVs)**.
* Identify the top EV manufacturers by vehicle count.
* Analyze the most popular EV models.
* Understand EV adoption trends across model years.
* Analyze the geographical distribution of EVs by state.
* Compare vehicles based on average electric range.
* Analyze **Clean Alternative Fuel Vehicle (CAFV) eligibility**.
* Create an interactive dashboard for easy exploration of EV data.

---

## 📊 Dashboard KPIs & Analysis

The dashboard includes the following key analyses:

### 1. Total Vehicles

Displays the total number of unique electric vehicles in the dataset.

### 2. BEV Vehicles

Shows the total number of **Battery Electric Vehicles (BEVs)**.

### 3. PHEV Vehicles

Shows the total number of **Plug-in Hybrid Electric Vehicles (PHEVs)**.

### 4. Average Electric Range

Calculates the average electric driving range of the vehicles.

### 5. Total Vehicles by Model Year

Visualizes EV adoption across different model years to identify growth patterns.

### 6. Top EV Manufacturers

Highlights the **Top N manufacturers** based on the number of electric vehicles.

A **Top N parameter** is included, allowing users to dynamically control the number of manufacturers displayed.

### 7. EVs by Model

Provides a model-level breakdown of electric vehicle population.

### 8. EVs by State

Uses a geographical map to visualize the distribution of electric vehicles across states.

### 9. CAFV Eligibility

Analyzes vehicles based on:

* CAFV Eligible
* CAFV Not Eligible
* CAFV Unknown

---

## 🗂️ Dataset

**Dataset:** Electric Vehicle Population Data

The dataset contains information about electric vehicles, including:

* VIN
* County
* City
* State
* Postal Code
* Model Year
* Make
* Model
* Electric Vehicle Type
* CAFV Eligibility
* Electric Range
* Base MSRP
* Legislative District
* Vehicle ID
* Vehicle Location
* Electric Utility
* Census Tract

---

## 🛠️ Tools & Technologies

* **Tableau**
* **Tableau Calculated Fields**
* **Tableau Parameters**
* **Tableau Filters**
* **Tableau Maps**
* **Data Visualization**
* **Data Analysis**

---

## 🔢 Calculated Fields

The project uses calculated fields to derive important metrics, including:

* Total Vehicles
* Total BEV Vehicles
* Total PHEV Vehicles
* BEV Percentage
* PHEV Percentage
* Average Electric Range

For example:

```text
Total Vehicles
COUNTD([DOL Vehicle ID])
```

BEV vehicles are calculated using conditional logic:

```text
COUNTD(
IF [Electric Vehicle Type] = "Battery Electric Vehicle (BEV)"
THEN [DOL Vehicle ID]
END
)
```

Similarly, PHEV vehicles are calculated using:

```text
COUNTD(
IF [Electric Vehicle Type] = "Plug-in Hybrid Electric Vehicle (PHEV)"
THEN [DOL Vehicle ID]
END
)
```

---

## 🎛️ Interactive Features

The dashboard provides interactive functionality through:

* Top N parameter
* Filters
* Interactive charts
* Geographic map
* Manufacturer-level analysis
* Model-level analysis
* EV type comparison
* CAFV eligibility analysis

---

## 📈 Key Insights

The dashboard can be used to answer questions such as:

* How many electric vehicles are represented in the dataset?
* What is the distribution between BEVs and PHEVs?
* Which manufacturers have the highest number of EVs?
* Which EV models are most popular?
* How has EV adoption changed across model years?
* Which states have the highest EV population?
* What is the average electric range?
* What percentage of vehicles are CAFV eligible?

---

## 📁 Project Files

```text
Tableau-EV-Sales-Analysis/
│
├── Tableau EV Sales Analysis.twbx
└── README.md
```

The `.twbx` file contains the Tableau workbook and its packaged data extract.

---

## 🚀 How to Use

1. Download the `.twbx` Tableau workbook.
2. Open it using **Tableau Desktop**.
3. Navigate to the **Dashboard**.
4. Use the available filters and Top N parameter to explore the data.
5. Interact with the charts and map to discover EV trends.

---

## 💡 Skills Demonstrated

This project demonstrates practical skills in:

* Data visualization
* Exploratory data analysis
* Tableau dashboard development
* Calculated fields
* Parameters
* Filters
* KPI development
* Geographic visualization
* Comparative analysis
* Data storytelling
* Business-oriented dashboard design

---

## 👩‍💻 Author

**Aksayalaxme Umapathy**

M.Sc. Physics | Aspiring Data Analyst

**Tools:** Excel | SQL | Python | Power BI | Tableau
