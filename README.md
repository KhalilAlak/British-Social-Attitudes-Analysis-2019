---

# 📊 British Social Attitudes Survey 2019

### **End-to-End Data Science Analysis (R Project)**

<p align="left">
  <img src="https://img.shields.io/badge/R-Tidyverse-blue?logo=r" />
  <img src="https://img.shields.io/badge/Analysis-Statistical%20%26%20ML-green" />
  <img src="https://img.shields.io/badge/Data-UK%20BSA%202019-orange" />
  <img src="https://img.shields.io/badge/Author-Khalil%20Alakbarzade-lightgrey" />
</p>

---

## 📌 Overview

This repository contains a full **end-to-end data science workflow** analysing the
**British Social Attitudes Survey 2019**, focusing on:

* Poverty & welfare opinions
* Political attitudes
* Demographic patterns (age, education, income)
* Public trust, spending priorities, and fraud perception

The project replicates **real consulting work** for HM Treasury, following the
workflow taught in the University of Sheffield module *IJC437 – Introduction to Data Science*.

---

## 🔍 Project Highlights

### **1. Data Preparation**

* Importing respondent-level survey data
* Converting all special missing codes to proper `NA`
* Cleaning, filtering, and validation

### **2. Feature Engineering**

* Recoding age into policy-friendly bands (18–34, 35–54, 55–64, 65+)
* Reshaping categorical variables
* Preparing data for modelling

### **3. Exploratory Data Analysis**

* Age–education distributions
* Demographic frequency tables
* Histograms and descriptive summaries

### **4. Statistical Testing**

* χ² test: **Age vs Education**
* Correlation analysis across political & social attitude variables

### **5. Machine Learning Models**

#### **Linear Regression**

Predicting perceived welfare fraud levels (`NatFrEst`) from:

* Political ideology
* Income level

#### **Logistic Regression**

Binary classification:
**“Increase taxes & spend” vs “Don’t increase taxes & spend”**

✔️ Achieved **95% prediction accuracy**

### **6. Visualisation**

* Heatmaps (Party ID × Social Media News Use, Spending Priorities)
* Correlation matrix (ggplot2 + corrplot)
* Boxplots (education vs age group)

---

## 🧠 Key Results (Short Summary)

* **Strong association between age and education** (χ², p < 0.001).
* **Political leaning** and **income** significantly predict fraud perception.
* **Logistic model** accurately predicts tax-spending attitudes.
* Clear grouping patterns in **Party ID, social media habits, and spending priorities**.

---

## 🛠️ Tools & Libraries

* **R:** tidyverse, ggplot2, corrplot, tidyr
* **Git & GitHub**
* **Markdown** for documentation

---

## 📁 Repository Structure

```
British-Social-Attitudes-Analysis-2019/
│
├── data/               # Raw data files (not included in repo)
├── scripts/            # R scripts (cleaning, EDA, modeling)
│    └── analysis.R
│
├── README.md           # Documentation
├── .gitignore          # Ignoring data, logs, temporary files
└── LICENSE             # Project license (MIT)
```

---

## ▶️ How to Run the Project

Open RStudio and run:

```r
source("scripts/analysis.R")
```

Make sure your dataset is placed inside the `data/` folder.

---

## 👤 Author

**Khalil Alakbarzade**
MSc Data Science – University of Sheffield
GitHub: [@KhalilAlak](https://github.com/KhalilAlak)

---

## 📄 License

This project is released under the **MIT License** — feel free to build on it.

<<<<<<< HEAD
---
=======
---
>>>>>>> 5cb6b9ef0bf1f6a5fc3aa7ca5a8d33d82a5fb59c
