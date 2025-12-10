---

## 1️⃣ Fix the merge conflict in `README.md`

In your project folder:

```bash
cd ~/British-Social-Attitudes-Analysis-2019
```

1. **Open `README.md` in an editor** (VS Code example):

   ```bash
   code README.md
   ```

   or, with nano:

   ```bash
   nano README.md
   ```

2. Inside the file you’ll see conflict markers like:

   ```text
   <<<<<<< HEAD
   ...your local version...
   =======
   ...GitHub version...
   >>>>>>> 5cb6b9e...
   ```

3. **Delete everything** in the file and replace it with the new README I give you below.

4. Save & close the editor.

5. Then run:

   ```bash
   git status          # should show “modified: README.md”
   git add README.md
   git commit -m "Resolve README merge conflict"
   git push origin main
   ```

After that, the conflict is gone and your local + GitHub are in sync.

---

## 2️⃣ New, cleaner README you can paste

Replace the whole file with this:

````markdown
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
````

> **Note:** The raw dataset is not included in the public repo.
> Place your local `.tab` file into `data/` before running the analysis.

---

## ⚙️ Tools & Packages

This project uses:

* **R** (tidyverse ecosystem)

  * `tidyverse` – data wrangling & plotting
  * `ggplot2` – visualisations
  * `corrplot` – correlation matrix visualisation
* **Git & GitHub** – version control and portfolio hosting
* **Markdown** – documentation

---

## 🚀 How to Run the Analysis

1. Clone the repository:

   ```bash
   git clone https://github.com/KhalilAlak/British-Social-Attitudes-Analysis-2019.git
   cd British-Social-Attitudes-Analysis-2019
   ```

2. Put the BSA 2019 `.tab` file into the `data/` folder (same name used in `scripts/analysis.R`).

3. Open R / RStudio and run:

   ```r
   source("scripts/analysis.R")
   ```

4. The script will:

   * Clean and transform the data
   * Run EDA and statistical tests
   * Fit linear & logistic regression models
   * Produce plots for heatmaps and the correlation matrix

---

## 🔍 Key Findings (Summary)

* **Age & education** show a strong association (large chi-square, p < 0.001).
* **Fraud perception (`NatFrEst`)** is influenced by both political orientation and income level.
* The **logistic model** predicting “Increase taxes & spend” vs “Don’t increase” achieves high accuracy on the test set.
* Party identification, spending priorities, and media habits show clear patterns in the heatmaps.

(Exact numbers are documented in `scripts/analysis.R` and the output.)

---

## 👤 Author

**Khalil Alakbarzade**
MSc Data Science, University of Sheffield

If you have questions or suggestions, feel free to open an issue or contact me via GitHub.

```

---

If you want, next I can also:

- suggest a `.gitignore` specific for R projects (Rproj, .Rhistory, etc.)
- help you add a nice LICENSE (MIT or Apache 2.0) and commit that too.
::contentReference[oaicite:0]{index=0}
```
