# Practical Machine Learning – Course Project  
Human Activity Recognition Using Random Forests

This repository contains my submission for the **Practical Machine Learning** course project (Coursera / Johns Hopkins University).  The objective is to build a predictive model that classifies the *manner* in which a barbell exercise was performed using accelerometer data from wearable sensors.

---

## Project Files
- `pml_project.Rmd` — main analysis  

## Data

The training and testing data were downloaded from the Coursera assignment page:

- Training: https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv  
- Testing: https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv  

The data come from the Human Activity Recognition project at PUC-Rio.

## Model

A Random Forest model was trained using the `caret` package.  
The final model was fitted on all cleaned training data and used to generate predictions for the 20 test cases.

## Results

The model achieved **very high accuracy** on the validation set  
(using a 70/30 split of the cleaned training data).

## How to Knit

Open `pml_project.Rmd` in RStudio and click:

**Knit → Knit to HTML**

## Reproducibility

- R version 4.x  
- Libraries: `caret`, `randomForest`, `dplyr`, `ggplot2`  
- Seed: `set.seed(12345)` 
