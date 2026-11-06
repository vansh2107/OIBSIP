
# Email Spam Detection Using Machine Learning

## Project Overview

This project was developed as part of the **Oasis Infobyte Data Science Internship**.

The objective is to build machine learning models that classify text messages into two categories:

- **Spam:** Unwanted or promotional messages.
- **Ham:** Legitimate messages.

The project uses Natural Language Processing (NLP), TF-IDF feature extraction, and supervised machine learning algorithms.

**Dataset clarification:** Although the internship task is titled Email Spam Detection, this implementation uses the SMS Spam Collection dataset recommended by the task instructions. Therefore, the experiment demonstrates SMS spam classification.

## Dataset

**Dataset:** SMS Spam Collection  
**Source:** UCI Machine Learning Repository  
**Dataset URL:** https://archive.ics.uci.edu/dataset/228/sms+spam+collection

The dataset contains 5,574 labelled messages:

| Category | Messages |
|---|---:|
| Ham | 4,825 |
| Spam | 747 |
| Total | 5,574 |

The dataset is distributed as a tab-separated text file named `SMSSpamCollection`.

## Technologies Used

- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK
- WordCloud
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Exploration
- Loaded the SMS Spam Collection dataset.
- Examined the dataset structure.
- Analysed the distribution of spam and ham messages.

### 2. Text Preprocessing
- Converted messages to lowercase.
- Removed punctuation, numbers, and special characters.
- Removed English stopwords.
- Applied Porter stemming.

### 3. Exploratory Data Analysis
- Compared message character lengths.
- Analysed word counts.
- Visualised message length distributions.

### 4. Feature Extraction
- Applied TF-IDF Vectorization.
- Used unigrams and bigrams.
- Limited the vocabulary to 5,000 features.
- Fitted the vectorizer only on training data to prevent data leakage.

### 5. Model Training
Two classification algorithms were implemented:

- Multinomial Naive Bayes
- Logistic Regression

The dataset was divided into 80% training data and 20% testing data using stratified sampling.

### 6. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### 7. WordCloud Visualisation

Generated separate WordCloud visualisations to identify frequently occurring words in spam and legitimate messages.

## Model Performance

| Metric | Multinomial Naive Bayes | Logistic Regression |
|---|---:|---:|
| Accuracy | 97.31% | 97.22% |
| Spam Precision | 100.00% | 100.00% |
| Spam Recall | 79.87% | 79.19% |
| Spam F1-score | 88.81% | 88.39% |

### Selected Model

**Multinomial Naive Bayes** performed slightly better across all four evaluation metrics.

Its confusion matrix showed:

- True Negatives: 966
- False Positives: 0
- False Negatives: 30
- True Positives: 119

The model achieved 97.31% accuracy and 79.87% spam recall on the test dataset.

## Project Structure

```text
DataScience-Task4-EmailSpamDetection/
│
├── data/
│   └── raw/
│       ├── SMSSpamCollection
│       └── readme
│
├── Screenshots/
│
├── Email_Spam_Detection.ipynb
├── README.md
└── requirements.txt
```

The `.venv` virtual environment is excluded from version control.

## Installation and Execution

### 1. Clone the repository

```bash
git clone https://github.com/vansh2107/OIBSIP.git
```

### 2. Navigate to the project directory

```bash
cd OIBSIP/DataScience-Task4-EmailSpamDetection
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the environment

Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Email_Spam_Detection.ipynb` and execute the notebook cells.

## Key Findings

- The dataset contains significantly more legitimate messages than spam messages.
- Spam messages generally contain more characters and words.
- Spam and legitimate messages exhibit different vocabulary patterns.
- Multinomial Naive Bayes achieved the best overall performance in this experiment.
- Improving spam recall remains an important opportunity for future work.

## Conclusion

This project demonstrates how Natural Language Processing and machine learning can be combined to identify spam messages.

Through data exploration, text preprocessing, TF-IDF feature extraction, model training, and evaluation, the project achieved 97.31% test accuracy using Multinomial Naive Bayes.

The experiment provides practical experience with text classification, machine learning evaluation, and visual data analysis.

---

**Internship:** Oasis Infobyte Data Science Internship  
**Project:** Email Spam Detection Using Machine Learning  
**Author:** Vansh Gandhi

