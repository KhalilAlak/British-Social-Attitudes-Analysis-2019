# 📊 British Social Attitudes 2019 – Poverty & Welfare Analysis

This repository contains an end-to-end data science project using the **British Social Attitudes Survey 2019**.  
The focus is on:

- Poverty and welfare attitudes  
- Political preferences and fraud perception  
- Demographic patterns (age, education, income)

The workflow follows a realistic **consulting task for HM Treasury** based on the IJC437 Week 10 practical.

---

## 🧱 Project Overview

1. **Data import & cleaning**
   - Load the open BSA 2019 poverty/welfare file
   - Recode special missing-value codes to proper `NA`
   - Create analysis-ready subsets

2. **Feature engineering**
   - Recode age into 4 groups (18–34, 35–54, 55–64, 65+)
   - Select and transform education, income, politics, and attitudes variables

3. **Exploratory data analysis**
   - Distributions (histograms, bar charts)
   - Cross-tabulations (age × education, party ID × media use)
   - Descriptive summaries

4. **Statistical modelling**
   - **Chi-square tests** for categorical associations  
   - **Linear regression** for fraud perception (`NatFrEst`)  
   - **Logistic regression** for tax & spending preferences (`TaxSpend`)

5. **Visualisation**
   - Boxplots  
   - Heatmaps for joint distributions  
   - Correlation matrix of key attitude variables

---

## 📁 Repository Structure

```text
British-Social-Attitudes-Analysis-2019/
├── data/
│   └── bsa2019_poverty_open.tab   # (not committed if large / confidential)
├── scripts/
│   └── analysis.R                 # main R analysis script
├── .gitignore
├── LICENSE
└── README.md
Note: The raw dataset is not included in the public repo.
Place your local .tab file into data/ before running the analysis.

⚙️ Tools & Packages
This project uses:

R (tidyverse ecosystem)

tidyverse – data wrangling & plotting

ggplot2 – visualisations

corrplot – correlation matrix visualisation

Git & GitHub – version control and portfolio hosting

Markdown – documentation

🚀 How to Run the Analysis
Clone the repository:

bash
Copy code
git clone https://github.com/KhalilAlak/British-Social-Attitudes-Analysis-2019.git
cd British-Social-Attitudes-Analysis-2019
Put the BSA 2019 .tab file into the data/ folder (same name used in scripts/analysis.R).

Open R / RStudio and run:

r
Copy code
source("scripts/analysis.R")
The script will:

Clean and transform the data

Run EDA and statistical tests

Fit linear & logistic regression models

Produce plots for heatmaps and the correlation matrix

🔍 Key Findings (Summary)
Age & education show a strong association (large chi-square, p < 0.001).

Fraud perception (NatFrEst) is influenced by both political orientation and income level.

The logistic model predicting “Increase taxes & spend” vs “Don’t increase” achieves high accuracy on the test set.

Party identification, spending priorities, and media habits show clear patterns in the heatmaps.

(Exact numbers are documented in scripts/analysis.R and the output.)


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