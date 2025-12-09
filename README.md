# Star Exams Clean Dataset

This repository contains an anonymized dataset of **5,203 users** from the _Star Exams_ Android application — an Ethiopian Grade 12 national exam preparation app developed by me and published on the Google Play Store.

📱 **App Link:**  
https://play.google.com/store/apps/details?id=com.easycodesolution.starexams

---

## 📊 Dataset Description

The file **`star_exams_clean_dataset.csv`** includes the following variables:

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

## 📁 Purpose

This dataset was prepared for academic statistical analysis in the course **Statistical Inference and Learning (CM90)** at Ca’ Foscari University.  
It supports investigations of digital access patterns, regional differences, and socioeconomic indicators based on smartphone characteristics.

---

## 🔗 Data Source

The original raw data were exported from my private **Firestore database** associated with the Star Exams application.  
This repository only contains a cleaned, anonymized version for research and reproducibility purposes.

---

## 📄 License

This dataset is released for **academic and research use only**. Redistribution for commercial purposes is not permitted.
