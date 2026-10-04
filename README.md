# Practical Machine Learning — Human Activity Recognition

A course project that applies supervised machine learning to wearable-sensor data from the **Weight Lifting Exercise Dataset**. The objective is to predict how a barbell exercise was performed (`classe`) from accelerometer measurements collected from the belt, forearm, arm and dumbbell.

## Project overview

The analysis covers data cleaning, removal of sparse and near-zero-variance predictors, exploratory analysis, model training and evaluation. The source analysis is written in R Markdown and the rendered report is included for convenient viewing.

## Repository contents

- [`CourseraMLproject.Rmd`](CourseraMLproject.Rmd) — complete R Markdown analysis.
- [`CourseraMLproject.html`](CourseraMLproject.html) — rendered project report.
- [`Project Details`](Project%20Details) — original assignment/project notes.

## Tools and methods

The analysis uses R and packages including `dplyr`, `caret`, `ggplot2`, `gmodels` and `nortest`. It includes preprocessing, exploratory visualization and supervised classification of the five exercise-quality classes.

## Data

The project uses the Weight Lifting Exercise Dataset originally supplied for the Coursera Practical Machine Learning course. The training and testing CSV files are referenced by the analysis but are not stored in this repository.

## Run locally

1. Download the training and testing data referenced in the R Markdown file.
2. Place `pml-training.csv` and `pml-testing.csv` in the working directory.
3. Open `CourseraMLproject.Rmd` in RStudio.
4. Install any missing R packages and knit the document.

## View the rendered report

GitHub stores the generated HTML report in this repository. For the best browser rendering, use an HTML preview service or download `CourseraMLproject.html` and open it locally.

## Notes

This repository preserves the original course analysis while providing clearer documentation around its purpose, workflow and reproducibility requirements.
