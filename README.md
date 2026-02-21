# Star Exams Clean Dataset and Statistical Analysis

This repository contains an anonymized dataset of **5,203 users** from the *Star Exams* Android application — an Ethiopian Grade 12 national exam preparation app developed by me and published on the Google Play Store.

📱 **App Link:**  
https://play.google.com/store/apps/details?id=com.easycodesolution.starexams

---

## 📊 Dataset Description

The file **`ethiopia_student_device_dataset.csv`** includes the following variables:

| Column | Description |
|--------|-------------|
| `user_id` | Random Firestore user UID (non-identifiable) |
| `city_clean` | Cleaned city name using fuzzy matching |
| `region` | Ethiopian administrative region |
| `device_raw` | Raw Android-reported device model |
| `device_brand` | Detected smartphone brand |
| `device_class` | Original budget/midrange/highend category |
| `device_range` | Final 3-tier classification: budget, midrange, upper_midrange |
| `device_model_norm` | Normalized model text |

All personal or sensitive information (name, phone number, password, etc.) has been removed during preprocessing. Only anonymized technical and geographic data are included.

---

## 📈 Statistical Analysis Files

This repository also includes the complete statistical analysis conducted in R:

| File | Description |
|------|------------|
| `star_exams_analysis.Rmd` | Fully documented R Markdown source code |
| `star_exams_analysis.html` | Compiled HTML report with results and visualizations |

The analysis includes:

- Exploratory data analysis (EDA)
- Confidence intervals for regional budget-device proportions
- Chi-square test of association
- Logistic regression (Addis Ababa vs Other Regions)
- Multinomial logistic regression
- LDA and QDA classification
- Cross-validation

All results are reproducible by running the `.Rmd` file.

---

## 🎓 Academic Purpose

This dataset and analysis were prepared for the course:

**Statistical Inference and Learning (CM90)**  
Ca’ Foscari University of Venice  

The project investigates digital access patterns and regional disparities in smartphone device characteristics among Ethiopian Grade 12 students using the Star Exams application.

---

## 🔬 Reproducibility

The R Markdown file loads the dataset directly from this repository to support transparency and reproducibility.

Running `star_exams_analysis.Rmd` will reproduce all statistical analyses, figures, tables, and model outputs included in the compiled HTML report.

---

## 🔗 Data Source

The original raw data were exported from my private **Firestore database** associated with the Star Exams application.

This repository contains only a cleaned and fully anonymized version for academic research purposes.

---

## 📄 License

This dataset and accompanying analysis are released for **academic and research use only**. Redistribution for commercial purposes is not permitted.
