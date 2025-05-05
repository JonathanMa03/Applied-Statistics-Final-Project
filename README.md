# Applied Statistics Final Project (S2025)

## Project Title
**Predictors of Academic Performance: The Role of Alcohol Consumption and Gender**

## Participants
Jonathan Ma

## Objective
This project investigates whether alcohol consumption (weekday vs. weekend) is predictive of student academic performance, and whether this effect is moderated by gender. We use a linear regression framework with interaction terms, controlling for over 30 demographic, behavioral, and socioeconomic variables.

---

## 🔍 Dataset

The dataset comes from the UCI Machine Learning Repository:

> P. Cortez and A. Silva. Using Data Mining to Predict Secondary School Student Performance.  
> In A. Brito and J. Teixeira Eds., Proceedings of 5th FUture BUsiness TEChnology Conference (FUBUTEC 2008), pp. 5-12, Porto, Portugal, April, 2008, EUROSIS, ISBN 978-9077381-39-7.  
> [https://archive.ics.uci.edu/ml/datasets/STUDENT+ALCOHOL+CONSUMPTION](https://archive.ics.uci.edu/ml/datasets/STUDENT+ALCOHOL+CONSUMPTION)

Two datasets were merged (`student-mat.csv` and `student-por.csv`) based on common student identifiers.

---

## Evaluation Rubric Checklist

### a. **Data set**  
✔️ Used a real-world dataset from UCI ML repository on Portuguese students' alcohol use and academic performance.

### b. **Preprocessing of data / data transformation**  
✔️ Transformed and merged datasets, created variables like `avggrades`, `mathgrades`, `portgrades`, and `alc_use`. Converted categorical variables using `factor()`.

### c. **Number of statistical concepts/methods used**  
✔️ Multiple regression models  
✔️ Interaction terms (`Dalc*sex`, `Walc*sex`)  
✔️ ANOVA model comparison  
✔️ Residual analysis  
✔️ Significance testing  
✔️ Normality and homoscedasticity tests (Shapiro-Wilk, Breusch-Pagan)

### d. **Visualizations**  
✔️ Residual plots, scatter plots, boxplots, and `geom_smooth` by gender/alcohol level

### e. **Project presentation**  
✔️ Published as an HTML report via GitHub Pages  
✔️ Clear structure: objectives, methods, results, and conclusion

### f. **Categorical variable vs. continuous variable**  
✔️ Treated `sex`, `school`, `guardian`, etc., as categorical  
✔️ Treated `avggrades`, `Dalc`, `Walc` as ordinal/continuous where appropriate

### g. **Which distributional assumption?**  
✔️ Tested normality (Shapiro-Wilk) and constant variance (Breusch-Pagan) on regression residuals

### h. **Exploratory data analysis**  
✔️ EDA conducted using summary statistics, correlation inspection, and visual patterns across alcohol levels and gender

### i. **R script**  
✔️ Code fully written in R, with reproducible RMarkdown document knitted to HTML

---

## 📊 Key Findings

- Weekend alcohol consumption (`Walc`) negatively predicts grades, especially among male students (`Walc:sexM`, p = 0.0018)
- Interaction terms significantly improve model fit (ANOVA p = 0.003)
- Gender moderates the effect of alcohol on academic performance
- The model satisfies core regression assumptions, with minor deviations noted

---

## 📎 Live Report

🔗 [View the full report (GitHub Pages)](https://jonathanma03.github.io/Applied-Statistics-Final-Project/AS_FinalProject.html)

---
