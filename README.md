# AutoSurvey

**AutoSurvey** is an open-source Python library designed to automate the statistical analysis of survey data. It allows users to quickly generate frequency tables, crosstabs, and descriptive statistics with minimal code. The project is part of a Google Summer of Code 2025 proposal under the Python Software Foundation.

##  Features

- Frequency tables for categorical variables
- Crosstabulations for comparing two variables
- Mean and standard deviation for numerical columns
- Planned: Hypothesis testing (t-test, chi-square)
- Planned: Confidence intervals
- Planned: Visualizations (bar charts, heatmaps)
- Optional: Streamlit-based user interface for non-programmers

##  Installation

This project is under development. You can clone the repository for testing and contribution:

```bash
git clone https://github.com/cansualltnts/AutoSurvey.git
cd AutoSurvey
pip install -r requirements.txt
```

##  Project Structure

```
AutoSurvey/
├── autosurvey/
│   └── analyzer.py
├── data/
│   └── example_survey.csv
├── tests/
│   └── test_analyzer.py
├── requirements.txt
└── README.md
```

##  Example Usage

```python
from autosurvey.analyzer import SurveyAnalyzer

# Load the dataset
analyzer = SurveyAnalyzer("data/example_survey.csv")

# Frequency analysis
print(analyzer.frequency("gender"))

# Crosstab analysis
print(analyzer.crosstab("gender", "education_level"))

# Descriptive statistics
print(analyzer.mean_std("age"))
```

Example `example_survey.csv` file:
```
gender,education_level,age
Female,Bachelor,23
Male,Master,31
Female,Bachelor,22
Male,PhD,40
Female,Master,27
```

## Technologies

- Python
- Pandas
- SciPy
- Statsmodels
- Matplotlib / Seaborn
- (Optional) Streamlit

## Purpose

The goal of this project is to support researchers, students, and educators who need quick and accurate statistical summaries of survey data — especially in educational and nonprofit environments where paid tools like SPSS or Excel may not be ideal.

## About the Developer

Developed by [@cansualltnts](https://github.com/cansualltnts)  
3rd-year Statistics Student – Ankara University  
Contributor for Google Summer of Code 2025 (Python Software Foundation)

## License

MIT License – Free to use, modify, and distribute.
