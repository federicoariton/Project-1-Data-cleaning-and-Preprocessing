# Titanic Dataset: Data Cleaning and Preprocessing

## Overview

This project demonstrates the data cleaning and preprocessing steps applied to the Titanic dataset to prepare it for analysis. The objective was to address missing values, correct data types, and handle outliers to ensure a reliable and analyzable dataset.

## Additional Resources

- More Information: For a detailed explanation of the project structure, methodologies, and findings, refer to the Full Project Report.[Full Project Report](https://github.com/federicoariton/Project-1-Data-cleaning-and-Preprocessing/blob/main/Data%20cleaning%20and%20Preprocessing%20Report%20pdf.pdf)

---

## Project Steps

### 1. Understanding the Dataset
- **Actions Taken**: 
  - Loaded the dataset and reviewed its structure.
  - Identified columns with missing values and encoded categorical data.
  - Noted discrepancies, such as numerical encoding in the `Embarked` column (e.g., 0.0, 1.0, 2.0 instead of C, Q, S).

---

### 2. Renaming and Correcting Columns
- **Objective**: Ensure clarity and correctness of column names.
- **Actions**:
  - Corrected the misnamed column `2urvived` to `Survived`.
  - Removed irrelevant columns such as `zero`, which contained no useful data.

---

### 3. Handling Missing Values
- **Objective**: Avoid errors due to missing data.
- **Actions**:
  - Focused on the `Embarked` column.
  - Analyzed the distribution of embarkation points and determined that 0.0, 1.0, and 2.0 represented `S` (Southampton), `C` (Cherbourg), and `Q` (Queenstown).
  - Imputed missing values in `Embarked` with 0.0 (Southampton), as it was the most common.

---

### 4. Data Type Conversion
- **Objective**: Optimize storage and processing by ensuring correct data types.
- **Actions**:
  - Converted `Pclass`, `Embarked`, and `Survived` columns to categorical data types.
  - Verified the conversions to confirm accuracy.

---

### 5. Handling Outliers
- **Objective**: Improve analysis accuracy by addressing extreme values.
- **Actions**:
  - Identified outliers in the `Fare` and `Age` columns using boxplots and histograms.
  - Applied the Interquartile Range (IQR) method to define acceptable value boundaries.
  - Capped outliers to the nearest acceptable values to minimize skewness.

---

### 6. Finalizing the Dataset
- **Actions**:
  - Saved the cleaned dataset as `cleaned_titanic_data.csv`.

---

## Key Takeaways
- A structured approach to cleaning and preprocessing ensures the dataset is accurate and ready for analysis.
- Techniques such as missing value imputation, data type conversion, and outlier handling are crucial for reliable data analysis.

---

## Files
- **`Data cleaning and Preprocessing Report.docx`**: Detailed steps and analysis of the cleaning process.
- **`cleaned_titanic_data.csv`**: Final cleaned dataset ready for analysis.

---

## Future Scope
This cleaned dataset can now be used for:
- Exploratory Data Analysis (EDA).
- Machine learning model training and evaluation.
- Further statistical analysis.

---

## Requirements
- Python (version 3.7 or later).
- Libraries: Pandas, NumPy, Matplotlib, Seaborn.

---

## How to Use
1. Clone the repository.
2. Load the cleaned dataset `cleaned_titanic_data.csv`.
3. Use the dataset for your analytical or modeling needs.

---

## Author
Federico Ariton  
[GitHub Profile](https://github.com/federicoariton)  
[LinkedIn Profile](https://www.linkedin.com/in/federico-ariton-090b18218/)

---

## License
This project is licensed under the MIT License.
