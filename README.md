📊 British Social Attitudes Survey 2019
End-to-End Data Science Analysis (R Project)

This repository contains a full data science workflow analysing the British Social Attitudes Survey (BSA) 2019, with a focus on poverty, welfare, political attitudes, social trust, and demographic patterns in Britain.

The project mirrors the structure of a professional consulting engagement for HM Treasury — from raw data → insights → statistical modelling → communication.

🚀 Project Overview

This analysis walks through the complete life-cycle of a data science project:

1️⃣ Data Import & Cleaning

Loading the official BSA 2019 dataset

Converting special missing-value codes (−1, 8, 9, 98, 99…)

Preparing variables for modelling

2️⃣ Feature Engineering

Recoding respondent age into policy-friendly groups

Handling education categories

Creating binary classes for logistic regression

Structuring variables for statistical models

3️⃣ Exploratory Data Analysis

Age distributions

Education patterns

Cross-tabulations

Demographic insights

4️⃣ Statistical Testing

Chi-square tests (age × education association)

Correlation analysis (political attitudes, spending views, poverty perception)

5️⃣ Machine Learning Models

Linear regression: Predicting fraud perception (NatFrEst) using politics + income

Logistic regression: Predicting who supports “Increase taxes & spend”

Model accuracy evaluation (95% achieved)

6️⃣ Visualisations

Heatmaps

Correlation matrix

Histograms

Boxplots

7️⃣ Reporting & Interpretation

Interpreting model coefficients

Explaining relationships in clear policy language

Turning findings into insights for stakeholders

📁 Project Structure
📦 British-Social-Attitudes-Analysis-2019
│
├── data/
│   └── bsa2019_poverty_open.tab      # raw dataset (excluded from GitHub)
│
├── scripts/
│   ├── analysis.R                    # full analysis pipeline
│   └── cleaning.R                    # data cleaning functions
│
├── README.md                         # this file
├── .gitignore                        # ignored files
└── LICENSE                           # project license

🧰 Tools & Libraries
R Packages

tidyverse — data wrangling

ggplot2 — visualisation

corrplot — correlation matrices

reshape2 / tidyr — heatmaps

stats — modelling (lm, glm, chisq.test)

Other Tools

Git & GitHub

Markdown

📌 Key Findings

📍 1. Age strongly predicts education levels
→ Chi-square test: p < 0.001

📍 2. Political beliefs significantly influence fraud perception (NatFrEst)
→ Political variables explain ~22% of variation alone
→ Adding income increases model explanatory power

📍 3. Logistic model accurately predicts tax-and-spend attitudes
→ Accuracy: 95.8%

📍 4. Clear relationships exist between media habits, spending priorities, and party ID

▶️ How to Run the Analysis

Open R or RStudio and run:

source("scripts/analysis.R")


Make sure the dataset is placed inside the data/ folder.

👤 Author

Khalil Alakbarzade
MSc Data Science — University of Sheffield
📍 Sheffield, United Kingdom
🔗 GitHub: https://github.com/KhalilAlak

📄 License

This project is released under the MIT License.
See the LICENSE file for details.
