# Human Activity Recognition with Machine Learning

A supervised machine-learning project using wearable-sensor data from the **Weight Lifting Exercise Dataset** to predict exercise quality (`classe`).

## Primary workflow

[`human_activity_recognition.Rmd`](human_activity_recognition.Rmd) is the audited source. It downloads the public course data when needed, creates a stratified internal hold-out split **before** data-dependent feature filtering, learns sparse/NZV predictor removal from the training partition only, applies the resulting schema unchanged to held-out and quiz data, and trains a 500-tree Ranger Random Forest with cross-validation.

## Repository contents

- [`human_activity_recognition.Rmd`](human_activity_recognition.Rmd) — audited R Markdown workflow.
- [`human_activity_recognition.html`](human_activity_recognition.html) — historical rendered course report; it may not reflect the current audited source.
- [`archive/legacy_course_analysis.Rmd`](archive/legacy_course_analysis.Rmd) — original submission retained for provenance.
- [`data/README.md`](data/README.md) — data-source and schema notes.
- [`R-packages.txt`](R-packages.txt) — direct R dependencies.
- [`docs/assignment_notes.md`](docs/assignment_notes.md) — original assignment notes.

## Reproducibility improvements

The legacy workflow filtered training and quiz data independently and used position-based column removal. The audited workflow instead creates the hold-out split first, learns missingness and near-zero-variance decisions only from the internal training partition, and verifies that every selected predictor exists before scoring held-out or quiz data. It also replaces a very small Random Forest with a more stable 500-tree model and removes normality testing that is not an assumption of Random Forest classification.

## Data

The two public course CSV files are downloaded automatically into `data/` if missing. See [`data/README.md`](data/README.md).

## Run locally

1. Install the packages listed in [`R-packages.txt`](R-packages.txt).
2. Open `human_activity_recognition.Rmd` in RStudio.
3. Run or knit the document from top to bottom.

## Scope

This is an educational human-activity-recognition project maintained as a reproducible machine-learning portfolio example.
