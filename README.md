📊 British Social Attitudes Survey 2019
End-to-End Data Science Analysis (R Project)
<p align="left"> <img src="https://img.shields.io/badge/R-Tidyverse-blue?logo=r" /> <img src="https://img.shields.io/badge/Analysis-Statistical%20%26%20ML-green" /> <img src="https://img.shields.io/badge/Data-BSA%202019-orange" /> <img src="https://img.shields.io/badge/Author-Khalil%20Alakbarzade-lightgrey" /> </p>
📌 Overview

This repository contains a complete end-to-end data science project analysing the
British Social Attitudes Survey 2019 (BSA).

The analysis focuses on:

Poverty & welfare attitudes

Political ideology

Demographics (age, education, income)

Trust, spending priorities, and fraud perception

This mirrors real consulting work for HM Treasury, following the workflow from the
University of Sheffield module IJC437 – Introduction to Data Science.

🔍 Project Highlights
1. Data Preparation

Importing large survey dataset

Converting special missing codes → proper NA

Cleaning & validation

2. Feature Engineering

Re-coding age groups into policy-friendly bands

Handling categorical variables

Preparing modelling datasets

3. Exploratory Data Analysis

Age × Education distributions

Demographic summaries

Visual inspection (histograms, tables, etc.)

4. Statistical Testing

Chi-square test: Age vs Education

Correlation analysis across political & social attitudes

5. Machine Learning Models
Linear Regression

Predicting welfare fraud perception (NatFrEst) using:

Political ideology

Income level

Logistic Regression

Binary classification:
Increase Taxes & Spend (1) vs Don’t Increase Taxes & Spend (0)

✔️ Achieved ~95% accuracy on the test set.

6. Visualisation

Heatmaps (Party ID × Social Media News; Spending Priorities × SMNews)

Correlation matrix

Boxplots (Age Group vs Education)

📁 Repository Structure
British-Social-Attitudes-Analysis-2019/
│
├── data/                     # Raw dataset (NOT included in repo)
│    └── bsa2019_poverty_open.tab  # Place your .tab file here
│
├── scripts/
│    └── analysis.R           # Main R analysis script
│
├── README.md                 # Project documentation
├── .gitignore                # Ignore data, logs, temp files
└── LICENSE                   # MIT License


📌 Note: The raw dataset is not included for size/privacy.
Place your .tab file inside the data/ folder before running the script.

🛠️ Tools & Libraries

This project uses:

R (tidyverse ecosystem)

tidyverse — data wrangling & plotting

ggplot2 — visualisations

corrplot — correlation matrices

tidyr / dplyr — reshaping & wrangling

Git & GitHub

Version control

Portfolio hosting

Markdown

Documentation

▶️ How to Run the Analysis

Clone the repository:

git clone https://github.com/KhalilAlak/British-Social-Attitudes-Analysis-2019.git


Open RStudio and run:

source("scripts/analysis.R")


Ensure your dataset is inside the data/ folder.

🧠 Key Findings (Short Summary)

Age is strongly associated with education (χ², p < 0.001).

Political ideology + income significantly predict perceived fraud levels.

Logistic model predicting tax-spending attitudes achieved ~95% accuracy.

Clear structure between Party ID, social media use, and spending priorities.

👤 Author

Khalil Alakbarzade
MSc Data Science – University of Sheffield
GitHub: @KhalilAlak

📄 License

Released under the MIT License — free to use, modify, and build on.
