# Heart Disease Dataset Analysis

## Overview
This project is undertaken as part of a formative assignment to analyze a dataset of medical records using unsupervised learning techniques, with the goal of identifying patients at high risk of developing heart disease. The analysis utilizes a dataset from the UCI Machine Learning Repository, containing 303 instances across 14 attributes including demographic data, medical history, and a target variable that indicates the presence or absence of heart disease.

## Dataset
The Heart Disease dataset sourced from the UCI Machine Learning Repository (UCI ID: 45) comprises data from multiple centers and countries. The dataset is instrumental in distinguishing the presence of heart disease based on various patient attributes.

### Attributes
- `age`: Age of the patient in years.
- `sex`: Gender of the patient (1 = male, 0 = female).
- `cp`: Chest pain type (values ranging from 1 = typical angina to 4 = asymptomatic).
- `trestbps`: Resting blood pressure (in mm Hg on admission to the hospital).
- `chol`: Serum cholesterol level in mg/dl.
- `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false).
- `restecg`: Resting electrocardiographic results (0 = normal, up to 2 = showing probable left ventricular hypertrophy).
- `thalach`: Maximum heart rate achieved.
- `exang`: Exercise-induced angina (1 = yes, 0 = no).
- `oldpeak`: ST depression induced by exercise relative to rest.
- `slope`: The slope of the peak exercise ST segment.
- `ca`: Number of major vessels colored by fluoroscopy (0-3).
- `thal`: Type of thalassemia (3 = normal, 6 = fixed defect, 7 = reversible defect).
- `target`: Presence of heart disease (0 = absence, 1-4 = presence).

## Analysis Steps
### Data Loading and Preprocessing
- Loaded the dataset into a Pandas DataFrame.
- Conducted exploratory data analysis (EDA) to understand the distribution of variables and handle missing values.

### Feature Engineering
- Imputed missing values using median values for numeric columns where applicable.
- Scaled features and encoded categorical variables to prepare data for clustering.

### Unsupervised Learning Techniques
- Applied K-means clustering, hierarchical clustering, and DBSCAN to segment patients based on their medical history.
- Utilized PCA and t-SNE for visualizing the data clusters to gain deeper insights into the relationships between attributes.

### Gaussian Mixture Models
- Implemented Gaussian Mixture Models (GMMs) to identify risk factors associated with heart disease.

### Evaluation
- Evaluated the performance of clustering algorithms using the silhouette score and Davies-Bouldin index.
- Compared different clustering algorithms to determine the most effective in identifying high-risk patients.

## Conclusion
The analysis provided significant insights into the patterns associated with heart disease. Potential next steps include refining models and integrating more sophisticated machine learning techniques to enhance predictive accuracy.

## Dependencies
- Python 3.x
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

## Repository Contents
- `Heart_Disease_UCI.ipynb`: Jupyter Notebook containing all the analysis, code, and visualizations.

## How to Use
1. Clone this repository.
2. Ensure all dependencies are installed.
3. Run the Jupyter Notebook to see the analysis.

