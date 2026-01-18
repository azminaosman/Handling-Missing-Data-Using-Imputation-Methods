# Handling Missing Data in Administrative Records Using Imputation Methods

## 📌 Overview

Administrative data plays a vital role in research, policy development, and operational decision-making. However, these datasets often contain missing values due to incomplete reporting, data entry errors, or system limitations. If not handled properly, missing data can lead to biased results and reduced analytical reliability.

This project explores practical and effective approaches to handling missing data using imputation techniques. By comparing both simple and advanced methods, the study aims to identify strategies that improve data quality while preserving the original characteristics of the data.

---

## ❓ Why This Matters

In real-world data projects, missing values are unavoidable—especially in large administrative and operational datasets. How missing data is handled can significantly influence analytical results, business decisions, and policy outcomes.

This study demonstrates practical approaches to improving data quality rather than discarding valuable information. It highlights the importance of choosing appropriate imputation techniques to ensure analyses remain accurate, reliable, and trustworthy—skills that are essential for data analysts, data scientists, and decision-makers working with imperfect real-world data.

---

## 🎯 Project Goals

- Understand how missing data affects administrative datasets  
- Compare commonly used imputation techniques  
- Evaluate how dataset size and missingness level influence imputation performance  
- Identify reliable methods for maintaining data accuracy and integrity  

---

## 🧪 Methodology

To simulate real-world administrative data scenarios, a synthetic clinical dataset was generated containing **20 numerical variables** such as BMI, blood pressure, and glucose levels.

### Experimental Setup

**Dataset Sizes**
- Small: 100 records  
- Medium: 3,000 records  
- Large: 50,000 records  

**Missing Data Mechanism**
- Missing Completely at Random (MCAR)

**Missingness Levels**
- 5%  
- 20%  
- 50%

---

## 🧩 Imputation Methods Compared

- **Mean Imputation**  
  Simple and fast, but sensitive to outliers

- **Median Imputation**  
  More robust to outliers than mean imputation

- **K-Nearest Neighbors (KNN)**  
  Estimates missing values using similarity between observations

- **Multiple Imputation by Chained Equations (MICE)**  
  An advanced, iterative approach that models relationships between variables

---

## 📊 Evaluation Metrics

Each imputed dataset was compared with the original complete dataset using:

- **Normalized Root Mean Squared Error (NRMSE)** to measure imputation accuracy  
- **Distribution analysis** to assess preservation of the original data structure  

---

## 🔍 Key Findings

- Larger datasets consistently resulted in better imputation accuracy  
- **MICE** achieved the best performance across all dataset sizes and missingness levels  
- **KNN** performed well, particularly at lower missingness levels  
- Simple methods (mean and median) became less reliable as missingness increased and tended to distort data distributions  

These findings indicate that while simple imputation techniques are easy to implement, advanced methods are more effective for maintaining data quality in complex administrative datasets.

---

## ✅ Conclusion

This project highlights the importance of selecting appropriate imputation techniques when working with incomplete administrative data. Advanced methods such as **MICE** provide more accurate and reliable results, especially when data quality is critical for analysis and decision-making. The findings support the use of robust imputation strategies in real-world administrative and clinical data applications.

---

## 🛠 Tools & Technologies

- Python  
- scikit-learn (`SimpleImputer`, `KNNImputer`, `IterativeImputer`)  
- Statistical evaluation using NRMSE  
- Data simulation and visualization  

---

## 📚 Publication

Osman, N. A., Yaacob, S., & Mohd Azmi, N. F. (2025). Handling missing data in administrative records through 
imputation methods for data quality improvement. International Journal of Business and Technology Management, 7(9), 297
308 https://doi.org/10.55057/ijbtm.2025.7.9.23.

