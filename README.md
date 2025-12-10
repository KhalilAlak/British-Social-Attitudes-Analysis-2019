📊 British Social Attitudes Survey 2019 – Data Science Analysis

This repository contains an end-to-end data science project analysing the British Social Attitudes Survey 2019, focusing on poverty, welfare, political attitudes, and demographic patterns.

The project simulates real consulting work for HM Treasury, following the structure of:

Data import & cleaning

Missing-value handling

Feature transformation (e.g., age recoding)

Exploratory data analysis

Statistical testing (Chi-square, correlations)

Machine learning models

Linear regression

Logistic regression

Visualisations (heatmaps, correlation matrix)

Summarising findings

🔧 Tools Used

R (tidyverse, ggplot2, corrplot, reshape2 or tidyr::pivot_longer)

Git & GitHub

Markdown

📁 Project Structure
data/       # raw data (not included)
scripts/    # R analysis code
README.md
.gitignore

📈 Key Results

Strong association between age and education level (χ² p < 0.001).

Political leaning and income impact fraud perception (NatFrEst).

Logistic model predicting “Increase taxes & spend” achieved 95% accuracy.

Strong patterns linking Party ID, spending priorities, and media habits.

🚀 How to Run
source("scripts/analysis.R")

📩 Contact

Created by Khalil Alakbarzade
MSc Data Science – University of Sheffield