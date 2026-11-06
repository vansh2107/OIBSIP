# Oasis Infobyte Data Science Internship

A collection of data science and machine learning projects completed as part of the **Oasis Infobyte Internship Program**.

This repository contains three projects covering exploratory data analysis, statistical insights, data visualization, natural language processing, and machine learning classification.

**Intern:** Vansh Gandhi  
**Internship Track:** Data Science  
**Organization:** Oasis Infobyte  
**GitHub Repository:** [OIBSIP](https://github.com/vansh2107/OIBSIP)

---

## Projects Overview

| Task | Project | Domain | Key Technologies |
|---|---|---|---|
| Task 1 | Iris Flower Classification | Machine Learning – Classification | Python, Pandas, Scikit-learn, Matplotlib, Seaborn |
| Task 2 | Unemployment Analysis with Python | Exploratory Data Analysis | Python, Pandas, NumPy, Matplotlib, Seaborn |
| Task 4 | Email Spam Detection | Natural Language Processing – Classification | Python, Pandas, NLTK, Scikit-learn, WordCloud |

---

## 1. Iris Flower Classification

**Project Folder:** `DataScience-Task1-IrisFlowerClassification`

### Objective
Build machine learning classification models to identify Iris flower species based on their physical measurements.

### Work Performed
- Loaded and explored the Iris dataset.
- Examined dataset dimensions, data types, and missing values.
- Performed exploratory data analysis using visualizations.
- Analyzed relationships between flower measurements and species.
- Split the dataset into training and testing sets.
- Trained and compared multiple classification algorithms.
- Evaluated models using classification metrics.

### Models Implemented
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest

### Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 93.33% |
| K-Nearest Neighbors | 93.33% |
| Decision Tree | 93.33% |
| Random Forest | 90.00% |

**Selected Model:** Logistic Regression

Logistic Regression was selected as the primary model due to its competitive performance and simplicity.

---

## 2. Unemployment Analysis with Python

**Project Folder:** `DataScience-Task2-UnemploymentAnalysis`

### Objective
Analyze unemployment trends in India, explore regional differences, and investigate changes during the COVID-19 period.

### Work Performed
- Loaded and inspected unemployment datasets.
- Examined missing values, data types, and descriptive statistics.
- Analyzed unemployment across Indian regions.
- Compared rural and urban observations.
- Visualized monthly unemployment trends.
- Investigated unemployment changes around the COVID-19 period.
- Examined correlations between unemployment, employment, and labour participation.

### Dataset Overview

| Metric | Value |
|---|---:|
| Valid observations | 740 |
| Regions covered | 28 |
| Urban observations | 381 |
| Rural observations | 359 |
| Date range | May 2019 – June 2020 |

### Key Findings

- Overall average unemployment rate: **11.79%**.
- Tripura recorded the highest regional average unemployment rate in the analysis.
- Unemployment increased substantially during April and May 2020.
- Average unemployment was approximately 9.51% before the COVID-19 cutoff and 17.77% from March 25, 2020 onward.
- The difference between these averages was approximately 8.26 percentage points.

**Key Takeaway:** The analysis highlights significant changes in India's unemployment patterns during the COVID-19 period, alongside regional variations.

---

## 3. Email Spam Detection with Machine Learning

**Project Folder:** `DataScience-Task4-EmailSpamDetection`

### Objective
Develop a machine learning system that classifies text messages as spam or ham (legitimate messages) using natural language processing techniques.

### Dataset
The project uses the UCI SMS Spam Collection dataset.

**Important:** Although the internship task is titled Email Spam Detection, the selected dataset contains SMS messages. The project transparently uses this dataset to demonstrate spam classification.

Dataset size: **5,574 messages**

| Class | Messages | Percentage |
|---|---:|---:|
| Ham | 4,825 | 86.56% |
| Spam | 747 | 13.40% |

### Work Performed
- Loaded and examined the SMS Spam Collection dataset.
- Analyzed class distribution.
- Preprocessed text through lowercasing, punctuation removal, stopword removal, and stemming.
- Analyzed message length and word count.
- Converted text into numerical features using TF-IDF.
- Applied stratified training and testing splits.
- Trained and compared two classification algorithms.
- Evaluated models using accuracy, precision, recall, F1-score, and confusion matrices.
- Generated separate WordCloud visualizations for spam and ham messages.

### Models Implemented
- Multinomial Naive Bayes
- Logistic Regression

### Results

| Metric | Multinomial Naive Bayes | Logistic Regression |
|---|---:|---:|
| Accuracy | 97.31% | 97.22% |
| Spam Precision | 100.00% | 100.00% |
| Spam Recall | 79.87% | 79.19% |
| Spam F1-score | 88.81% | 88.39% |

**Selected Model:** Multinomial Naive Bayes

Multinomial Naive Bayes achieved slightly better overall performance on the test dataset.

The evaluation also highlights why recall matters in spam detection: missed spam messages can reach the user's inbox even when a classifier has high accuracy.

---

## Repository Structure

```text
OIBSIP/
│
├── DataScience-Task1-IrisFlowerClassification/
│   ├── Iris_Flower_Classification.ipynb
│   ├── README.md
│   ├── requirements.txt
│   └── Screenshots/
│
├── DataScience-Task2-UnemploymentAnalysis/
│   ├── data/
│   │   └── raw/
│   ├── Unemployment_Analysis.ipynb
│   ├── README.md
│   ├── requirements.txt
│   └── Screenshots/
│
├── DataScience-Task4-EmailSpamDetection/
│   ├── data/
│   │   └── raw/
│   ├── Email_Spam_Detection.ipynb
│   ├── README.md
│   ├── requirements.txt
│   └── Screenshots/
│
├── .gitignore
└── README.md
```

Each project directory contains its own documentation, dependencies, notebook, and relevant supporting files.

---

## Technologies Used

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Natural Language Processing:** NLTK
- **Text Feature Extraction:** TF-IDF
- **Word Visualization:** WordCloud
- **Development Environment:** Jupyter Notebook, VS Code
- **Version Control:** Git and GitHub

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/vansh2107/OIBSIP.git
```

### 2. Navigate to the repository

```bash
cd OIBSIP
```

### 3. Open an individual project

For example:

```bash
cd DataScience-Task1-IrisFlowerClassification
```

### 4. Set up the Python environment

```bash
python -m venv .venv
```

Activate the environment:

**Windows PowerShell:**

```powershell
.venv\Scripts\Activate.ps1
```

### 5. Install project dependencies

```bash
pip install -r requirements.txt
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the corresponding `.ipynb` notebook and execute the cells.

**Note:** Each project has its own `requirements.txt`. Run the installation command from the relevant project directory. Follow the individual README for dataset and execution details.

---

## Learning Outcomes

Through these projects, I gained practical experience in:

- Data cleaning, preprocessing, and exploratory data analysis.
- Statistical analysis and data interpretation.
- Data visualization and communicating insights.
- Supervised machine learning classification.
- Model training, comparison, and evaluation.
- Natural language processing and text preprocessing.
- TF-IDF feature extraction.
- Working with real-world datasets.
- Organizing projects and maintaining code using Git and GitHub.

---

## Acknowledgement

I would like to thank **Oasis Infobyte** for providing the opportunity to work on practical Data Science projects as part of its internship program.

---

## Author

**Vansh Gandhi**

- GitHub: [@vansh2107](https://github.com/vansh2107)
- Repository: [OIBSIP](https://github.com/vansh2107/OIBSIP)

---

*This repository represents my practical learning and implementation of Data Science concepts through the Oasis Infobyte Internship Program.*
