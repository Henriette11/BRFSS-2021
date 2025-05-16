# BRFSS 2021  
**DTSC 650: Data Analytics In R**  


## 📋 Project Overview

This project analyzes the 2021 Behavioral Risk Factor Surveillance System (BRFSS) dataset to answer public health questions using tidyverse in R and pipelines in Quarto. It covers:

1. **Data Loading & Cleaning**  
   - Load `BRFSS2015_650.csv` via `read_csv()`  
   - Handle special codes (e.g. `88 → 0` for `MENTHLTH`, recode exercise/alc variables)  
   - Keep dataframes for analysis (avoid multiple copies)

2. **Descriptive Summaries**  
   - Q1: Count excellent general health (`GENHLTH == 1`)  
   - Q2: Average exercise frequency by stroke status  
   - Q3: Mean & SD of mental health (`MENTHLTH`) by caregiving status  
   - Q4: Median age at diabetes diagnosis in Pennsylvania

3. **Statistical Modeling**  
   - Q5: Linear regression predicting poor mental‐health days from marital status  
   - Q6: Summarise mean poor‐mental‐health days by marital status  
   - Q7: Mean & SD of poor‐mental‐health by stroke status among uninsured  
   - Q8: ANOVA of exercise frequency by marital status  
   - Q9: Variance in drinking days by primary exercise type (men only)

---

## 🚀 How to Run

1. **Set working directory** in RStudio:  
   Session → Set Working Directory → To Source File Location  
2. **Install & load tidyverse** (once):  
   ```r
   install.packages("tidyverse")  
   library(tidyverse)
