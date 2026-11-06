# Iris Flower Classification Using Machine Learning

## 1. Project Overview

This project focuses on developing a Machine Learning classification model to predict the species of an Iris flower based on its physical measurements.

The model classifies flowers into three species:

- Iris Setosa
- Iris Versicolor
- Iris Virginica

The project demonstrates the complete Machine Learning workflow, including data loading, exploratory data analysis, visualisation, feature analysis, model training and evaluation.

## 2. Dataset Information

The project uses the built-in Iris dataset provided by Scikit-learn.

**Dataset characteristics:**

- Total observations: 150
- Numerical features: 4
- Target classes: 3
- Missing values: 0

**Input features:**

1. Sepal Length (cm)
2. Sepal Width (cm)
3. Petal Length (cm)
4. Petal Width (cm)

**Target variable:** Iris species.

No external dataset download is required.

## 3. Technologies and Libraries

- Python 3.12.7
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## 4. Project Workflow

### 4.1 Dataset Loading

Loaded the Iris dataset directly from Scikit-learn and converted it into a Pandas DataFrame.

### 4.2 Exploratory Data Analysis

Performed:

- Dataset structure and shape inspection.
- Data type inspection.
- Missing-value analysis.
- Descriptive statistical analysis.
- Species distribution analysis.

### 4.3 Data Visualisation

Created:

- Pairplot to examine relationships between numerical features.
- Four box plots to analyse feature distributions across species.

### 4.4 Feature Selection Analysis

Compared feature measurements across the three species.

Petal length and petal width demonstrated particularly strong differences between species.

### 4.5 Train-Test Split

Divided the dataset into:

- Training data: 80%
- Testing data: 20%

Stratified sampling was applied to preserve the species distribution.

### 4.6 Model Training

Implemented four classification algorithms:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Decision Tree
4. Random Forest

StandardScaler was used with Logistic Regression and KNN.

### 4.7 Model Evaluation

Evaluated the classifiers using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrices
- Classification reports

### 4.8 Feature Coefficient Analysis

Examined Logistic Regression coefficients to understand the contribution of individual features to the classification scores.

## 5. Model Performance

The following results were obtained using the 20% test dataset.

| Model | Accuracy | Weighted Precision | Weighted Recall | Weighted F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 93.33% | 93.33% | 93.33% | 93.33% |
| K-Nearest Neighbors | 93.33% | 94.44% | 93.33% | 93.27% |
| Decision Tree | 93.33% | 93.33% | 93.33% | 93.33% |
| Random Forest | 90.00% | 90.24% | 90.00% | 89.97% |

## 6. Best-Performing Model

Logistic Regression and Decision Tree achieved joint top performance, with an accuracy of 93.33% and a weighted F1-score of 93.33%.

Logistic Regression was selected as the primary model for the final demonstration because of its relatively simple classification approach and competitive performance.

## 7. Key Findings

- The Iris dataset contains 150 complete observations with no missing values.
- Petal length and petal width are particularly useful for distinguishing Iris species.
- All four models correctly classified every Setosa observation in the test set.
- Logistic Regression, KNN and Decision Tree achieved 93.33% accuracy.
- Random Forest achieved 90.00% accuracy.

## 8. Project Structure

```text
DataScience-Task1-IrisFlowerClassification/
│
├── Iris_Flower_Classification.ipynb
├── README.md
├── requirements.txt
│
└── screenshots/
    ├── dataset_overview.png
    ├── pairplot.png
    ├── boxplots.png
    ├── model_comparison.png
    └── confusion_matrices.png
```

## 9. Installation and Execution

### Prerequisites

- Python 3.12.7 or compatible Python version.
- Visual Studio Code or Jupyter Notebook.

### Step 1: Clone the repository

```bash
git clone https://github.com/vansh2107/OIBSIP.git
```

### Step 2: Navigate to the project directory

```bash
cd OIBSIP/DataScience-Task1-IrisFlowerClassification
```

### Step 3: Create a virtual environment

```bash
python -m venv .venv
```

### Step 4: Activate the environment

Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### Step 5: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 6: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Iris_Flower_Classification.ipynb` and execute the notebook cells.

## 10. Conclusion

This project demonstrates the application of supervised Machine Learning algorithms to a multiclass classification problem.

Through exploratory data analysis, feature visualisation and model evaluation, the project identifies useful patterns in Iris flower measurements and compares the performance of four classification algorithms.

Logistic Regression was selected as the primary model, achieving 93.33% accuracy on the test dataset.

---

**Internship:** Oasis Infobyte

**Track:** Data Science

**Project:** Task 1 — Iris Flower Classification