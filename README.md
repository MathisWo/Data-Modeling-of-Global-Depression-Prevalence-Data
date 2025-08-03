# 🌍 Data Modeling of Global Depression Prevalence Data

This project models a small database for global depression prevalence data using R and PostgreSQL.
The goal is to structure and clean the data with R and create a dimensional data model with PostgresSQL.
This  builds the foundation for further analysis and visualization with SQL and R.

---

## 🧠 Project Summary

- **Data Source**: IHME / Global Burden of Disease dataset (citation at the end of this file)
- **Focus**: Prevalence of depression by country and year
- **Tools**:
  - R (for cleaning, transformation, export)
  - PostgreSQL (for modeling a small data warehouse structure)
  - pgAdmin (for SQL table management, data import)
  - RMarkdown (for documentation and reporting)

---

## 📁 Repository Structure

Data-Modeling-of-Global-Depression-Prevalence-Data/

📄README.md

📄prevalence_analysis.Rmd      # RMarkdown with full workflow

📄prevalence_analysis.html     # Rendered HTML report

📄where_to_find_the_data.md    # Describes where and how to get the data


---

## 📦 Tools

- **R (4.4.2)**
- **RStudio (2024.12.0)**
- **PostgreSQL**
- **pgAdmin4 (9.3)**
- **R Packages**:
  - tidyverse (2.0.0)

---

## 🗄️ SQL Table Structure

Three tables are created using a star schema design:

- 'country_dim(country_id, country)'
- 'year_dim(year_id, year)'
- 'prevalence_fact(prevalence_id, prevalence, country_id, year_id)'

Each table can be populated by importing the corresponding '.csv' file in **pgAdmin**.

---

## ✍️ Author

**MathisWo**  
M.Sc. Psychology | Aspiring Data Analyst  
[LinkedIn](https://www.linkedin.com/in/mathis-wobst-b37125360/?locale=en_US)

---

The data used in this project is publicly available and is from the **Institute for Health Metrics and Evaluation (IHME)**.

Citation:
  Global Burden of Disease Collaborative Network.
  Global Burden of Disease Study 2021 (GBD 2021) Results.
  Seattle, United States: Institute for Health Metrics and Evaluation (IHME), 2022.
  Available from https://vizhub.healthdata.org/gbd-results/..
