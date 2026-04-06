# Agricultural Data Cleaning & Integration Pipeline

## Overview

This project demonstrates a complete data preparation workflow, including extracting, merging, and cleaning agricultural data from multiple relational tables into a single analysis-ready dataset.

The dataset originates from an SQLite database containing multiple tables covering geographic, weather, soil, and farm management features. These tables were integrated into a unified dataset using SQL joins and processed using Python.

---

## Project Workflow

### 1. Data Extraction

* Connected to an SQLite database
* Retrieved data from multiple tables:

  * geographic_features
  * weather_features
  * soil_and_crop_features
  * farm_management_features

### 2. Data Integration

* Joined all tables using a common key: `Field_ID`
* Executed a single SQL query to efficiently combine datasets

### 3. Data Cleaning

Identified and corrected several real-world data issues:

* **Swapped Columns**

  * Fixed incorrect placement of `Annual_yield` and `Standard_yield`

* **Inconsistent Crop Names**

  * Standardized text (lowercase, trimmed whitespace)
  * Corrected spelling errors (e.g., *maeze → maize*)

*  **Invalid Elevation Values**

  * Converted negative elevation values to positive

* **Data Type Corrections**

  * Ensured numerical fields were properly formatted

* **General Cleaning**

  * Removed duplicates
  * Validated dataset consistency

---

## Tools & Technologies

* Python
* Pandas
* SQL (SQLite)
* SQLAlchemy

---

## Key Skills Demonstrated

* Data extraction and integration using SQL
* Data cleaning and preprocessing with Pandas
* Handling real-world data inconsistencies
* Data validation and transformation
* Preparing datasets for analysis and machine learning

---

## Outcome

The final dataset is clean, structured, and ready for:

* Exploratory Data Analysis (EDA)
* Data visualization
* Predictive modeling

---

## ⚠️ Disclaimer

**This repository contains a copy of my original work and is intended solely for portfolio demonstration. I do not take responsibility for any distribution, reproduction, or misuse of this content by third parties.**

---

## Future Improvements

* Build predictive models for crop yield
* Perform advanced statistical analysis
* Develop interactive dashboards

---

## Author

*Mike Bwisa Mwasame - ALX Alumni*

---

⭐ If you found this project useful, feel free to star the repository!
