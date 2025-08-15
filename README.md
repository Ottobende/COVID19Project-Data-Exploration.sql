# COVID-19 Data Exploration – SQL Project

## 📌 Overview
This project performs **data exploration and analysis** on global COVID-19 datasets using SQL.  
It demonstrates advanced SQL techniques such as:
- **Joins**
- **Common Table Expressions (CTEs)**
- **Temporary Tables**
- **Window Functions**
- **Aggregate Functions**
- **Views**
- **Data Type Conversions**

The goal is to extract meaningful insights from COVID-19 statistics, including infection rates, death percentages, and population impacts.

---

## 📂 Dataset
The project uses two main tables:
- **`CovidDeaths`** – Contains data on COVID-19 cases, deaths, population, and locations.
- **`CovidVaccinations`** – Contains vaccination-related data per country.

**Source:** [Our World in Data – Coronavirus Dataset](https://ourworldindata.org/coronavirus)

---

## 🔍 Key Analysis Performed
1. **Initial Data Selection**
   - Filtering relevant data where `continent` is not null.
   - Sorting by location and date.

2. **Case Fatality Rate**
   - Calculating death percentage:  
     ```sql
     (total_deaths / total_cases) * 100 AS DeathPercentage
     ```

3. **Infection Rate per Population**
   - Percentage of population infected:
     ```sql
     (total_cases / population) * 100 AS PercentPopulationInfected
     ```

4. **Highest Infection Rates**
   - Identifying countries with the highest infection percentage.

5. **Highest Death Counts**
   - Finding countries with the highest COVID-19 death tolls.

6. **Vaccination Analysis** *(if available)*
   - Tracking progress and percentage of populations vaccinated.

---

## 🛠 SQL Concepts Demonstrated
- Filtering and Ordering (`WHERE`, `ORDER BY`)
- Grouping and Aggregations (`GROUP BY`, `MAX`, `SUM`)
- Mathematical Calculations in queries
- Common Table Expressions (CTEs)
- Window Functions for running totals
- Joins between deaths and vaccination tables
- Creating Views for reusable queries

---

## 🚀 How to Use
1. Download the SQL script: [`Covid 19 Project.sql`](Covid%2019%20Project.sql)
2. Import the COVID-19 dataset into your SQL Server database (or compatible RDBMS).
3. Run the queries step-by-step to explore the insights.

---

## 📊 Example Insights
> - The **United States** had a case fatality rate above **3%** during certain periods.  
> - Some countries reported infection rates exceeding **20% of their total population**.  
> - Vaccination drives showed significant variance across continents.

---

## 🖼 Query Output Examples

### 1. Death Percentage Over Time
![Death Percentage Over Time](images/death_percentage_over_time.png)

### 2. Highest Infection Rates by Country
![Highest Infection Rates](images/highest_infection_rates.png)

### 3. Vaccination Progress
![Vaccination Progress](images/vaccination_progress.png)

*(Replace the placeholder images above with screenshots from your query results.)*

---

## 📜 License
This project is for **educational purposes**.  
Data courtesy of *Our World in Data*.
