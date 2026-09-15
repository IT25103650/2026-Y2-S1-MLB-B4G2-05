# Tourist Satisfaction Prediction & Segmentation Using Machine Learning

**Group ID:** 2026-Y2-S1-MLB-B4G2-05
**Module:** IT2011 – Artificial Intelligence and Machine Learning
**Domain:** Tourism & Hospitality Analytics

## Project Overview

Tourism operators can lose repeat visitors and referrals when tourists leave dissatisfied. By the time a negative review appears, it may already be too late to improve that visitor’s experience.

This project uses a dataset of approximately **100,000 domestic tourism trips** to build a data-driven system that helps identify dissatisfaction risk and understand the factors associated with tourist satisfaction.

The dataset includes:

* Visitor demographics such as age, gender, and home province
* Attraction details such as category, quality tier, and location
* Trip information including ticket price, spending, visit duration, season, and holiday timing
* Group-tour information such as transport mode and group fees

The target variable is:

```text
satisfaction_level
```

with three categories:

```text
Neutral
Satisfied
Very Satisfied
```

## Objectives

The main objectives of this project are to:

1. Clean and preprocess the raw dataset.
2. Handle structurally missing values, inconsistent labels, outliers, and categorical variables.
3. Identify factors associated with tourist satisfaction using statistical techniques such as Chi-Square testing and correlation analysis.
4. Build a compact, model-ready feature set using feature selection, encoding, scaling, and PCA.
5. Prepare the dataset for future supervised classification and unsupervised clustering.
6. Ultimately support:

   * Tourist satisfaction prediction
   * Dissatisfaction risk identification
   * Tourist segmentation into behavioural personas
   * Service quality improvement
   * More effective tourism marketing

## Assigned Dataset

**Dataset:** `tourism_recommendation_dataset_en.csv`

The original dataset is stored in:

```text
data/raw/tourism_recommendation_dataset_en.csv
```

## Preprocessing Techniques

The following preprocessing techniques were applied during Progress Review I:

* **Missing Data Handling**
* **Categorical Encoding**

  * Label Encoding
  * One-Hot Encoding
  * Target Encoding
* **Outlier Removal**

  * IQR Method
* **Normalization / Scaling**

  * StandardScaler
* **Feature Selection**

  * Chi-Square Filter Method
* **Dimension Reduction**

  * Principal Component Analysis (PCA)

## Group Member Roles

| Member   | Assigned Technique            |
| -------- | ----------------------------- |
| Member 1 | Missing Data Handling         |
| Member 2 | Categorical Encoding          |
| Member 3 | Outlier Removal               |
| Member 4 | Normalization / Scaling       |
| Member 5 | Feature Selection             |
| Member 6 | Dimension Reduction using PCA |

Each member is responsible for explaining their preprocessing technique, why it was needed, how it was implemented, the output produced, and the related before-and-after EDA.

## Project Structure

```text
2026-Y2-S1-MLB-B4G2-05/
│
├── README.md
│
├── data/
│   ├── raw/
│   │   └── tourism_recommendation_dataset_en.csv
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
        ├── output_after_missing_data.csv
        ├── output_after_feature_selection.csv
        ├── output_after_outlier_removal.csv
        ├── output_after_encoding.csv
        ├── output_after_scaling.csv
        └── final_processed_dataset.csv
```

## Integrated Preprocessing Pipeline

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
PCA Dimension Reduction
        ↓
Final Processed Dataset
```

## Exploratory Data Analysis

EDA was used to understand the dataset and compare the data before and after preprocessing.

Visualizations include:

* Histograms
* Boxplots
* Count plots
* Correlation analysis
* Before-and-after preprocessing comparisons

EDA outputs are stored in:

```text
results/eda_visualizations/
```

## How to Run the Project

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

Then run all cells from top to bottom.

## Main Python Libraries

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

These libraries are used for data cleaning, preprocessing, EDA, categorical encoding, feature selection, scaling, and PCA.

## Final Output

The final machine-learning-ready dataset is stored in:

```text
results/outputs/final_processed_dataset.csv
```

The integrated `group_pipeline.ipynb` combines all preprocessing techniques into one complete workflow.

The processed dataset will later be used for **tourist satisfaction prediction and tourist segmentation using machine-learning techniques**.
