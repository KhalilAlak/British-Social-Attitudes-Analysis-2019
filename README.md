
# 📊 British Social Attitudes Survey 2019 – Data Science Analysis

This project presents an **end‑to‑end data science workflow in R**, using the  
**British Social Attitudes (BSA) Survey 2019**, focusing on public attitudes toward  
poverty, welfare, political ideology, income, and social behaviour.

The analysis simulates real consulting work for **HM Treasury**, following the  
structure of the University of Sheffield module *IJC437 – Introduction to Data Science*.

---

## 🚀 Project Workflow

### **1. Data Preparation**
- Importing survey `.tab` dataset  
- Converting special missing codes into `NA`  
- Cleaning, filtering, and validation checks  

### **2. Feature Engineering**
- Recoding age into 4 policy‑friendly bands  
- Handling categorical scales  
- Preparing modelling‑ready datasets  

### **3. Exploratory Data Analysis (EDA)**
- Age × education distribution  
- Demographic frequency tables  
- Histograms and descriptive summaries  

### **4. Statistical Testing**
- **Chi‑square test**: Age vs Education  
- **Correlation matrix** across attitude & political variables  

### **5. Machine Learning Models**

#### **Linear Regression**
Predicting perceived welfare fraud (`NatFrEst`) using:
- Political ideology  
- Income level  

#### **Logistic Regression**
Binary classification:  
**Increase taxes & spend (1)** vs **Don’t increase (0)**  
✔ Achieved **~95% accuracy**

### **6. Visualisations**
- Heatmaps (Party ID × Social Media News Use, Spending Priorities)  
- Correlation matrix (corrplot)  
- Boxplots (education vs age group)

---

## 📁 Repository Structure

```
British-Social-Attitudes-Analysis-2019/
│
├── data/                     # Raw dataset (NOT committed)
│   └── bsa2019_poverty_open.tab
│
├── scripts/                  # R scripts for EDA & modelling
│   └── analysis.R            # Main workflow script
│
├── README.md                 # Project documentation
├── .gitignore                # Local files ignored
└── LICENSE                   # MIT License
```

> **Note:** Dataset is NOT included for privacy/size reasons.  
Add your `.tab` file into the `data/` folder before running the script.

---

## 🛠 Tools & Packages

### **R Packages**
- tidyverse (dplyr, tidyr, readr)
- ggplot2
- corrplot
- tibble

### **Other Tools**
- Git & GitHub  
- RStudio  
- Markdown  

---

## ▶️ How to Run

Open RStudio and run:

```r
source("scripts/analysis.R")
```

Make sure:
1. Your `.tab` dataset is placed in `/data`
2. All packages are installed
3. You run the script from the project root directory

---

## 📌 Key Findings

- **Strong relationship** between age and education (χ², p < 0.001)  
- **Political ideology + income** influence welfare‑fraud perception  
- Logistic model achieves **~95% accuracy**  
- Clear grouping patterns in Party ID, SMNews, and spending preferences  

---

## 👤 Author

**Khalil Alakbarzade**  
MSc Data Science – University of Sheffield  
GitHub: https://github.com/KhalilAlak

---

## 📄 License

Distributed under the **MIT License**.
