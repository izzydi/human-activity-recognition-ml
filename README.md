# Human Activity Recognition with Machine Learning

A supervised machine-learning project using wearable-sensor data from the **Weight Lifting Exercise Dataset**. The objective is to predict how a barbell exercise was performed (`classe`) from accelerometer measurements collected from the belt, forearm, arm and dumbbell.

## Project overview

The analysis covers data cleaning, removal of sparse and near-zero-variance predictors, exploratory analysis, model training and evaluation. The source analysis is written in R Markdown and the rendered report is included for convenient review.

## Repository contents

- [`human_activity_recognition.Rmd`](human_activity_recognition.Rmd) — complete R Markdown analysis.
- [`human_activity_recognition.html`](human_activity_recognition.html) — rendered project report.
- [`docs/assignment_notes.md`](docs/assignment_notes.md) — original assignment notes retained for provenance without cluttering the project root.

## Tools and methods

The analysis uses R and packages including `dplyr`, `caret`, `ggplot2`, `gmodels` and `nortest`. It includes preprocessing, exploratory visualization and supervised classification of five exercise-quality classes.

## Data

The project uses the Weight Lifting Exercise Dataset originally supplied for the Coursera Practical Machine Learning course. The training and testing CSV files are referenced by the analysis but are not stored in this repository.

## Run locally

1. Download the training and testing data referenced in the R Markdown file.
2. Place `pml-training.csv` and `pml-testing.csv` in the project directory.
3. Open `human_activity_recognition.Rmd` in RStudio.
4. Install any missing R packages and knit the document.

## View the rendered report

Download `human_activity_recognition.html` and open it in a browser for the complete rendered analysis.

## Notes

The original analytical work is preserved while the repository structure and naming have been cleaned for portfolio use.
