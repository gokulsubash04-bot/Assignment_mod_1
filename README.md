# 🏥 Healthcare Data Analysis and Insights

## 📌 Project Overview

The **Healthcare Data Analysis and Insights** project is an Excel-based data analysis project designed to analyze healthcare information such as patient health profiles, medical history, hospitalization details, and healthcare costs.

The project performs **data cleaning, data transformation, data integration, analysis, visualization, and dashboard creation** to identify meaningful patterns and relationships within the healthcare dataset.

---

## 🎯 Objectives

The main objectives of this project are:

- Clean missing and inconsistent healthcare data.
- Transform raw healthcare data into meaningful categories.
- Combine multiple healthcare tables using Customer ID.
- Analyze patient health conditions and medical history.
- Analyze healthcare charges based on different health conditions.
- Study relationships between age, BMI, HBA1C, and healthcare charges.
- Create interactive visualizations.
- Build a dashboard for easy interpretation of healthcare insights.

---

## 📂 Dataset

The project uses three main tables:

### 1. Customer Names
Contains customer identification and name information.

### 2. Medical Examinations
Contains medical information such as:

- BMI
- HBA1C
- Heart Issues
- Any Transplants
- Cancer History
- Number of Major Surgeries
- Smoker Status

### 3. Hospitalisation Details
Contains hospitalization and cost-related information such as:

- Customer ID
- Year
- Month
- Date
- Charges
- Hospital Tier
- City Tier
- State ID

---

## 🧹 Data Cleaning

The following cleaning operations were performed:

- Identified missing values represented by `?`.
- Missing month values were replaced with **Sep**.
- Missing year values were replaced with the **rounded average year**.
- Missing smoker values were filled using the **mode**.
- Missing Hospital Tier values were filled using the **mode**.
- Missing City Tier values were filled using the **mode**.
- Missing State ID values were replaced with **Unknown**.
- Customer ID values containing `?` were retained rather than fabricating customer IDs.

---

## 🔄 Data Transformation

### Name Splitting

The original names were separated into:

- Title
- First Name
- Last Name

### Major Surgeries

`NumberOfMajorSurgeries` was converted into numerical values.

`No major surgery` was represented as:

```text
0
