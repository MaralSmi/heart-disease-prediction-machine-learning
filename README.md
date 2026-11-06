# Heart Disease Prediction Using Machine Learning

**Exploratory Data Analysis, Classification, Dimensionality Reduction, and Model Evaluation**

## Project Overview

This repository presents an academic machine learning project focused on predicting the presence or absence of heart disease using patient-related clinical features.

The project was completed individually as the final assignment for the *Introduction to Artificial Intelligence* course in the B.Sc. Industrial Engineering program at Shahid Beheshti University.

The project covers data preprocessing, exploratory data analysis, feature importance, dimensionality reduction, clustering, and the comparison of supervised classification algorithms.

## Dataset

The analysis uses a heart disease dataset containing **918 observations and 12 columns**, including the target variable.

The target variable is `HeartDisease`, representing the presence or absence of heart disease.

The dataset includes the following features:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Fasting blood sugar
- Resting electrocardiogram results
- Maximum heart rate
- Exercise-induced angina
- Oldpeak
- ST slope

The dataset was provided by the course instructor for academic purposes. Its original source and redistribution permissions have not yet been verified.

**Note:** The original `heart.csv` dataset is not currently included in this repository. The notebook's saved outputs can be viewed without the dataset, but rerunning the analysis requires access to the data.

## Project Workflow

### 1. Data Preprocessing

- Examined numerical and categorical variables.
- Checked for missing values; none were identified in the dataset.
- Included imputation procedures for potential missing values.
- Encoded categorical variables using label encoding and one-hot encoding.
- Applied standard scaling to numerical features.

### 2. Exploratory Data Analysis (EDA)

- Visualized numerical feature distributions.
- Examined categorical feature frequencies.
- Created a correlation heatmap to explore relationships between variables.
- Investigated feature importance using a Decision Tree classifier.

### 3. Dimensionality Reduction

Applied **Principal Component Analysis (PCA)** to explore the dataset in a lower-dimensional feature space.

The project includes two-dimensional and three-dimensional visualizations.

### 4. Clustering

Applied **K-Means clustering** using different numbers of clusters, from two to five.

The clustering results were explored through PCA-based visualizations.

### 5. Classification Models

Four supervised classification algorithms were investigated:

| Model | Description |
|---|---|
| Decision Tree | Tree-based classification and feature importance analysis |
| Logistic Regression | Linear probabilistic classification |
| XGBoost | Gradient-boosted decision trees |
| Support Vector Machine (SVM) | Margin-based classification |

### 6. Model Evaluation

The models were compared using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC curves and Area Under the Curve (AUC)
- Execution time

The project used an **80/20 training-test split** with `random_state=42`.

## Results and Findings

The original experiment identified **Logistic Regression as the best-performing model according to AUC**.

The project report includes ROC curve visualizations comparing Logistic Regression, XGBoost, SVM, and Decision Tree.

These findings reflect the original academic experiment and should not be interpreted as evidence of clinical reliability.

## Technologies and Libraries

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- XGBoost

## Repository Contents

| File | Description |
|---|---|
| `maral_esmikhani_ML_FINAL_PROJECT_402236016.ipynb` | Original Jupyter Notebook containing the project code, visualizations, and saved outputs |
| `ML_Final_Project_Report_EN.pdf` | English project report describing the methodology, experiments, and findings |
| `maral_esmikhani_ML_FINAL_PROJECT_402236016.pdf` | Original Persian project report |
| `README.md` | Project documentation |

### Project Files and Reports

- [Jupyter Notebook](maral_esmikhani_ML_FINAL_PROJECT_402236016.ipynb)
- [English Project Report](ML_Final_Project_Report_EN.pdf)
- [Persian Project Report](maral_esmikhani_ML_FINAL_PROJECT_402236016.pdf)

## Reproducibility and Limitations

This repository preserves the original academic project and its documented results.

The Jupyter Notebook originally loads the dataset using a local Windows file path. To rerun the analysis on another computer, the dataset must first be obtained and the file path updated.

The original workflow also has methodological limitations:

- Some preprocessing operations were performed before the training-test split, creating a potential risk of **data leakage**.
- The reported performance metrics have not yet been independently revalidated using a leakage-safe preprocessing pipeline.
- The analysis is intended for educational purposes and is not a clinical diagnostic tool.

Potential future improvements include:

- Adding the original dataset after confirming its source and redistribution permissions.
- Replacing the local dataset path with a relative path.
- Implementing preprocessing through scikit-learn pipelines fitted only on the training data.
- Using cross-validation and further model validation.

## Academic Context

**Course:** Introduction to Artificial Intelligence  
**Institution:** Shahid Beheshti University, Tehran, Iran  
**Instructor:** Dr. Shahabeddin Nabavi  
**Project period:** Winter 1403 (Solar Hijri calendar)  
**Project type:** Individual academic assignment

## Author

**Maral Esmikhani**  
B.Sc. Industrial Engineering  
Shahid Beheshti University, Tehran, Iran

[GitHub Profile](https://github.com/MaralSmi)

---

*This project is intended for educational and academic portfolio purposes only.*
