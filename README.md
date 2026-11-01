# Predicting the Japa Syndrome: An Exploratory Machine Learning Study

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine_Learning-orange?logo=scikitlearn)
![Status](https://img.shields.io/badge/Project-Completed-success)

## 📌 Project Overview

The Japa phenomenon, commonly used to describe the movement of Nigerians abroad in search of better opportunities, has become an important social and economic issue in Nigeria.

This project explores the factors associated with Nigerians' intentions to leave the country and investigates whether machine learning models can predict respondents' intentions based on their survey responses.

Using data collected from 188 respondents, I conducted exploratory data analysis, statistical testing, and machine learning experiments to understand patterns in the responses and build predictive models.

The project was completed as part of the 3MTT mentorship programme.

## 🎯 Problem Statement

Many Nigerians consider relocating abroad for different reasons, including employment opportunities, education, security, and quality of life.

But what can survey data tell us about these intentions?

The central question guiding this project was:

**"Have you seriously considered leaving Nigeria within the next five years?"**

The aim was to explore the responses, identify possible patterns, and investigate whether machine learning could help predict respondents' answers.

## 🎯 Project Objectives

The objectives of this project were to:

- Explore the demographic characteristics of survey respondents.
- Understand patterns in respondents' intentions to leave Nigeria.
- Investigate possible relationships between demographic variables and migration intentions.
- Prepare and transform the data for machine learning.
- Build and compare different classification models.
- Evaluate model performance using appropriate evaluation metrics.
- Identify the limitations of the analysis and suggest areas for improvement.

## 📊 Dataset Description

The dataset was collected through a survey completed by 188 respondents.

It contained 36 columns before data preprocessing and feature engineering.

Some of the information collected included:

- Age
- Gender
- Marital status
- Educational qualification
- Employment status
- Income
- Family members living abroad
- Previous applications or attempts to relocate
- Intention to leave Nigeria within the next five years

### Dataset Overview

| Description | Value |
|---|---:|
| Number of responses | 188 |
| Original columns | 36 |
| Age group with the highest responses | 24–29 years |
| Female respondents | 107 |
| Male respondents | 81 |
| Largest state represented | Enugu |

**Note:** The processed modelling dataset contained 50 columns after encoding and feature engineering.

## 🛠️ Tools and Technologies

The following tools and Python libraries were used:

- **Python:** Programming language.
- **Pandas:** Data manipulation and cleaning.
- **NumPy:** Numerical computations.
- **Matplotlib:** Data visualisation.
- **Seaborn:** Statistical data visualisation.
- **Scikit-learn:** Data preprocessing, model building and evaluation.
- **Jupyter Notebook:** Development and documentation.

## 🔄 Project Workflow

The project followed these major steps:

### 1. Data Collection

Survey responses were collected from 188 participants to understand their experiences, demographic backgrounds, and intentions concerning migration.

### 2. Data Cleaning and Preprocessing

The dataset was inspected and prepared for analysis.

This involved:
- Checking for missing values.
- Inspecting data types.
- Handling categorical variables.
- Cleaning relevant text responses.
- Preparing features for machine learning.

### 3. Exploratory Data Analysis (EDA)

I explored the dataset to understand the characteristics of the respondents and identify patterns in their responses.

Some of the variables examined included age, gender, education, employment, income, and family connections abroad.

### 4. Statistical Analysis

Chi-square tests of independence were used to investigate possible associations between selected demographic variables and respondents' intentions to leave Nigeria.

The significance level was set at 0.05.

The results did not show statistically significant associations for the demographic variables tested at this significance level.

This does not establish that these factors have no relationship with migration intentions. It means the analysis did not provide sufficient statistical evidence of an association in this sample.

### 5. Feature Engineering

Categorical variables were transformed into numerical representations to make them suitable for machine learning.

MultiLabelBinarizer was also used to transform responses from multiple-selection questions into separate binary features.

### 6. Model Development

I experimented with four classification approaches:

- Logistic Regression
- Support Vector Machine (SVM)
- L1-Regularised Logistic Regression
- Random Forest Classifier

### 7. Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Class weighting was also explored to address the imbalance between the response classes.

## 📈 Model Performance

After experimenting with class weighting, the models produced the following results:

| Model | Accuracy | ROC-AUC |
|---|---:|---:|
| Logistic Regression | 63.2% | 0.740 |
| Support Vector Machine | 78.9% | 0.833 |
| L1 Logistic Regression | 60.5% | 0.755 |
| Random Forest | **89.5%** | **0.875** |

The Random Forest model achieved the highest accuracy and ROC-AUC among the evaluated models.

These results suggest that Random Forest performed best among the models tested in this experiment.

However, the results should be interpreted carefully because the dataset was relatively small and imbalanced.

## 🔍 Key Findings and Lessons

Some important lessons from this project include:

1. Data exploration is important before building predictive models. Understanding the dataset helps guide the modelling process.

2. Statistical tests do not always reveal significant relationships. Results should be interpreted based on the available evidence rather than personal assumptions.

3. Accuracy alone is not enough when evaluating an imbalanced classification problem. Other metrics, especially recall, precision, F1-score and ROC-AUC, provide additional information.

4. Different machine learning algorithms can produce different results on the same dataset.

5. A model's performance on a small survey dataset does not automatically mean it can generalise to the wider Nigerian population.

## ⚠️ Project Limitations

This project has some limitations:

- The dataset contains only 188 responses and may not represent the wider Nigerian population.
- Some demographic groups are more represented than others.
- The target classes are imbalanced.
- The findings are based on self-reported survey responses.
- Predictive performance may change when the model is tested on a larger and more diverse dataset.

The project should therefore be viewed as an exploratory study rather than a definitive explanation or prediction of migration behaviour across Nigeria.

## 🚀 Future Improvements

If I were to continue this project, I would like to:

- Collect more responses from a wider range of Nigerian states.
- Improve the representation of underrepresented groups.
- Explore additional feature selection techniques.
- Experiment with more classification algorithms.
- Conduct further model tuning and validation.
- Investigate additional factors that may influence migration intentions.

## 💻 How to Run This Project

To explore this project on your local machine:

**1. Clone the repository**

```bash
git clone https://github.com/chilotamchinecheremC/Emigration-intent-prediction.git

**2. Navigate to the project folder**

```bash
cd Emigration-intent-prediction
```

**3. Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**4. Launch Jupyter Notebook**

```bash
jupyter notebook
```

**5. Open the project notebook and run the cells.**

Replace the repository URL and notebook instructions with your actual file names and setup requirements.

## 🙏 Acknowledgements

I sincerely appreciate my 3MTT mentor for the guidance, feedback, patience, and encouragement throughout this project.

Special thanks to 3MTT and Deep Tech for providing the opportunity to learn and gain practical experience.

I also appreciate WesOnline for organising the mentorship sessions that made this learning experience possible.

Finally, thank you to everyone who participated in the survey and contributed to this project.

## 👩‍💻 Author

**Chinecherem Chilotam Catherine**

Data Science Learner | Mathematics Graduate | Aspiring Machine Learning Practitioner

- GitHub: [My GitHub Profile](https://github.com/chilotamchinecheremC)
- LinkedIn: [My LinkedIn Profile](https://www.linkedin.com/in/chinecheremchilotam/)

---

*This project was completed as part of the 3MTT mentorship programme. It represents a practical learning experience in data analysis, statistical testing, and machine learning.*
