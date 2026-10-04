# Legacy course analysis

`legacy_course_analysis.Rmd` preserves the original Practical Machine Learning course submission.

It is retained for provenance, but the audited workflow is [`../human_activity_recognition.Rmd`](../human_activity_recognition.Rmd). The original source filtered training and quiz datasets independently and used fragile position-based column removal, which could produce mismatched predictor schemas. The audited source derives feature selection from training data once and applies the same predictor names to every downstream dataset.

The root HTML file is a historical rendered report and may not reflect the current audited source.
