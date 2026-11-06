# Heart Disease Prediction Using Machine Learning

**Exploratory Data Analysis, Classification, Dimensionality Reduction, and Model Evaluation**

## Project Overview

This repository presents an academic machine learning project focused on predicting the presence or absence of heart disease using patient-related clinical features.

The project was completed individually as the final assignment for the *Introduction to Artificial Intelligence* course in the B.Sc. Industrial Engineering program at Shahid Beheshti University.

The project explores data preprocessing, exploratory data analysis, feature importance, dimensionality reduction, clustering, and the comparison of supervised classification algorithms.

## Dataset

The analysis uses a heart disease dataset containing **918 observations and 12 columns**, including the target variable.

The target is `HeartDisease`, representing the presence or absence of heart disease.

The dataset includes features such as:

- Age and sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Fasting blood sugar
- Resting electrocardiogram results
- Maximum heart rate
- Exercise-induced angina
- Oldpeak and ST slope

The dataset was provided for the academic project. Its original provenance should be confirmed before adding a formal dataset citation.

## Project Workflow

### 1. Data Preprocessing

- Examined numerical and categorical features.
- Checked for missing values; none were identified in the dataset.
- Included imputation procedures for potential missing values.
- Encoded categorical variables using label encoding and one-hot encoding.
- Applied standard scaling for analyses requiring normalized feature values.

### 2. Exploratory Data Analysis

- Visualized numerical feature distributions.
- Examined categorical feature frequencies.
- Created a correlation matrix to explore relationships between variables.
- Investigated feature importance using a decision tree classifier.

### 3. Dimensionality Reduction

Applied Principal Component Analysis (PCA) to visualize the data in a lower-dimensional space and examine explained variance.

### 4. Clustering

Applied K-Means clustering with different cluster counts, from two to five, and visualized the resulting clusters using three-dimensional PCA projections.

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
- Training and prediction execution time

The project used an 80/20 training-test split with `random_state=42`.

## Results and Findings

The reported model comparison identified **Logistic Regression as the best-performing model according to AUC** in the original experiment.

The report also includes ROC visualizations for Logistic Regression, XGBoost, SVM, and Decision Tree.

These findings describe the results of the academic experiment and should not be interpreted as evidence of clinical reliability.

## Technologies and Libraries

- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib and Seaborn
- scikit-learn
- XGBoost

## Repository Contents

| File | Description |
|---|---|
| `maral_esmikhani_ML_FINAL_PROJECT_402236016.ipynb` | Original Jupyter Notebook containing the project code and saved outputs |
| `ML_Final_Project_Report_EN.pdf` | English project report describing the methods, visualizations, and findings |
| `README.md` | Project documentation |

**[View the English Project Report](ML_Final_Project_Report_EN.pdf)**

**[Explore the Jupyter Notebook](maral_esmikhani_ML_FINAL_PROJECT_402236016.ipynb)**

## Reproducibility and Limitations

This repository preserves the original academic project.

The notebook uses a local file path to load `heart.csv`. To execute the analysis on another computer, the dataset must be available and its path must be updated.

The original workflow also has methodological limitations that should be considered before interpreting the reported performance:

- Some preprocessing operations were performed before the training-test split, creating a potential risk of data leakage.
- The reported metrics come from the original experimental setup and have not been independently revalidated using a leakage-safe preprocessing pipeline.
- The analysis is educational and is not intended for clinical diagnosis or medical decision-making.

Future improvements could include restructuring preprocessing with scikit-learn pipelines, adding cross-validation, and evaluating model performance on an independent test dataset.

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

*This project is intended for educational and research portfolio purposes only.*
