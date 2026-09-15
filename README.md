# 2026-Y2-S1-MLB-B4G2-05

## Tourism Recommendation Dataset – Data Preprocessing and EDA

### Project Overview

This project was completed for the **IT2011 – Artificial Intelligence and Machine Learning** module as part of the **Progress Review I – Data Preprocessing and Exploratory Data Analysis (EDA)**.

The main objective of the project is to prepare the assigned tourism recommendation dataset for machine learning by applying a complete data preprocessing pipeline.

The preprocessing techniques used in this project are:

1. Missing Data Handling
2. Feature Selection
3. Outlier Removal
4. Categorical Encoding
5. Normalization / Scaling
6. Dimensionality Reduction using PCA

Each preprocessing technique was completed individually by a group member and later integrated into one complete preprocessing pipeline.

---

## Assigned Dataset

**Dataset Name:** `tourism_recommendation_dataset_en.csv`

The dataset contains tourism-related information that can be used for developing a tourism recommendation system.

The original dataset is stored in:

```text
data/raw/tourism_recommendation_dataset_en.csv
```

During preprocessing, several intermediate datasets are generated after each preprocessing stage.

These include:

```text
output_after_missing_data.csv
output_after_feature_selection.csv
output_after_outlier_removal.csv
output_after_encoding.csv
output_after_scaling.csv
final_processed_dataset.csv
```

The final processed dataset is stored inside:

```text
results/outputs/
```

---

## Group Member Roles

| Member   | Assigned Preprocessing Technique   |
| -------- | ---------------------------------- |
| Member 1 | Missing Data Handling              |
| Member 2 | Categorical Encoding               |
| Member 3 | Outlier Removal                    |
| Member 4 | Normalization / Scaling            |
| Member 5 | Feature Selection                  |
| Member 6 | Dimensionality Reduction using PCA |

Each member is responsible for explaining:

- What their preprocessing technique does
- Why the technique was required for the dataset
- How the technique was implemented
- The output produced after preprocessing
- Before-and-after EDA visualizations
- Interpretation of the results

---

## Project Structure

```text
2026-Y2-S1-MLB-B4G2-05/
│
├── README.md
│
├── data/
│   ├── raw/
│   │   └── tourism_recommendation_dataset_en.csv
│   │
│   └── external/
│
├── notebooks/
│   ├── Member_1_Missing_Data_Handling.ipynb
│   ├── Member_2_Categorical_Encoding.ipynb
│   ├── Member_3_Outlier_Removal.ipynb
│   ├── Member_4_Normalization_Scaling.ipynb
│   ├── Member_5_Feature_Selection.ipynb
│   └── Member_6_Dimension_Reduction_PCA.ipynb
│
├── group_pipeline.ipynb
│
└── results/
    ├── eda_visualizations/
    ├── logs/
    └── outputs/
        └── final_processed_dataset.csv
```

---

## Preprocessing Pipeline

The integrated preprocessing pipeline follows this order:

```text
Original Dataset
      ↓
Missing Data Handling
      ↓
Feature Selection
      ↓
Outlier Removal
      ↓
Categorical Encoding
      ↓
Normalization / Scaling
      ↓
PCA Dimensionality Reduction
      ↓
Final Processed Dataset
```

## Jupyter Notebook

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Navigate to the project folder:

```bash
cd 2026-Y2-S1-MLB-B4G2-05
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
group_pipeline.ipynb
```

and run all cells from the beginning.

---

## Main Python Libraries

The project uses common Python data science and machine learning libraries including:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
```

These libraries are used for data loading, cleaning, visualization, feature preprocessing, scaling, encoding and PCA.

---

## Final Output

After completing all preprocessing stages, the final machine-learning-ready dataset is saved as:

```text
results/outputs/final_processed_dataset.csv
```

The integrated notebook `group_pipeline.ipynb` demonstrates how the individual preprocessing techniques are combined into one logical workflow.
