# Handling Missing Data in Administrative Records Using Imputation Methods

## 📌 Overview

Administrative data—such as records from hospitals, schools, or government agencies—is essential for research, policy decisions, and daily operations. However, these datasets often contain missing values due to incomplete reporting, human error, or system glitches. Ignoring these gaps can lead to misleading results and unreliable analyses.

Rather than simply deleting incomplete records, this project explores practical ways to fill in the blanks accurately using imputation techniques. By comparing simple methods (mean or median) with advanced approaches (KNN and MICE), we aim **to identify the most effective strategies for improving data quality**, ensuring datasets remain reliable, accurate, and useful for real-world decision-making

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

