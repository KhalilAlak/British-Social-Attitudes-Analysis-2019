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

This repository presents a complete **end-to-end data science workflow** using the  
**British Social Attitudes Survey 2019** dataset. The analysis focuses on:

- Poverty & welfare perceptions  
- Political attitudes  
- Income & education patterns  
- Trust, spending preferences, and fraud estimates  
- Social media news behaviour  

The project mirrors real consulting work for **HM Treasury**, following the structure taught in  
**IJC437 – Introduction to Data Science (University of Sheffield)**.

---

## 🔍 Project Highlights

### **1. Data Preparation**
- Importing raw survey data (`.tab`)
- Converting special BSA missing-value codes into proper `NA`
- Filtering invalid or incomplete responses

### **2. Feature Engineering**
- Recoding age into policy-friendly groups (18–34, 35–54, 55–64, 65+)
- Cleaning categorical variables  
- Preparing modelling-ready datasets  

### **3. Exploratory Data Analysis**
- Age × education distributions  
- Summary statistics  
- Histograms, frequency tables  

### **4. Statistical Testing**
- **Chi-square test**: strong association between age and education  
- Correlation exploration among political & social attitude variables  

### **5. Machine Learning Models**

#### **Linear Regression**
Predicting **NatFrEst** (Perception of welfare fraud) using:
- Political ideology (leftrigh, libauth, welfare2)
- Political engagement  
- Income level  

#### **Logistic Regression**
Binary classification for:
**Increase taxes & spend** vs **Don’t increase taxes & spend**

- Achieved **95% accuracy** on the test set.

### **6. Visualisation**
- Heatmaps (Party ID × SMNews, Spending Priorities)
- Correlation matrix  
- Boxplots (Education by Age Group)

---

## 🧠 Key Findings

- **Strong correlation** between **age** and **education** (χ², p < 0.001).  
- **Political leaning** and **income** significantly influence fraud perception.  
- Logistic regression accurately predicts tax-and-spend preferences.  
- Clear demographic patterns in **Party ID** and **social media news use**.  

---

## 🛠️ Tools & Libraries

- **R:** tidyverse, ggplot2, corrplot, tidyr  
- Git & GitHub  
- Markdown  

---

## 📁 Repository Structure

British-Social-Attitudes-Analysis-2019/
│
├── data/ # Raw data (NOT included in repo)
├── scripts/ # R scripts for EDA & modelling
│ └── analysis.R
│
├── README.md # Project documentation
├── .gitignore # Ignoring data & temp files
└── LICENSE # MIT License

yaml
Copy code

---

## ▶️ How to Run

1. Place the dataset (e.g., `bsa2019_poverty_open.tab`) into the `data/` folder  
2. Open RStudio  
3. Run:

```r
source("scripts/analysis.R")
👤 Author
Khalil Alakbarzade
MSc Data Science – University of Sheffield
GitHub: @KhalilAlak

📄 License
Released under the MIT License.
Feel free to use, adapt, or build on this project.