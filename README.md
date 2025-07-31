# Power Source Detection Case Study

## Project Overview
This case study focuses on detecting active power sources (Grid, Solar, Generator) in health facilities in Sierra Leone using voltage and frequency data collected by sensors. In many healthcare centers across sub-Saharan Africa, power is sourced from a combination of the national grid, solar panels, and diesel generators. Understanding which source is active at a given time enables better energy planning, cost tracking, and improved solar investment evaluations.

### Objective
Improve and evaluate machine learning approaches for identifying the active power source based on time-series sensor data. The goal is to replace or enhance the existing rule-based algorithm with a more robust, data-driven model.

## Folder Structure
```
├── documents/                         # Case study description and reference documents
│   └── Data Science Case Study 3.pdf
│
├── notebooks/                         # Jupyter notebooks from each contributor
│   ├── casestudy_edwin.ipynb
│   ├── casestudy_risper.ipynb
│   ├── casestudy_katherin.ipynb
│   └── casestudy_andrew.ipynb
│
├── README.md                          # Project overview and setup instructions
└── .gitignore                         # Git ignore file
```

## Collaboration Workflow
- Each team member will create their own branch using the format: `<firstname>_casestudy`
- Work independently in a personal notebook: `casestudy_<firstname>.ipynb`
- Merge via pull requests and review collaboratively

## Data Science Workflow
This case study follows a standard data science project pipeline:

### 1. Problem Understanding
- Review context and goals
- Understand sensor setup and the need for power source identification

### 2. Data Cleaning & Preparation
- Convert time to datetime objects
- Clean `respondent_id`, fix malformed entries
- Remove unknown or irrelevant power source labels
- Handle outliers and round voltage/frequency for consistency
- Extract time-based features (hour, day, date, etc.)

### 3. Exploratory Data Analysis (EDA)
- Univariate and bivariate analysis
- Time-series trends across hospitals and power sources
- Outlier detection and visual pattern identification

### 4. Feature Engineering
- Time-based features
- Aggregated statistics (rolling averages, hourly means)
- Possible signal processing if required

### 5. Modeling
- Train and evaluate multiple supervised models (e.g., decision trees, SVM, random forest)
- Use rule-based output as ground truth for evaluation

### 6. Evaluation
- Accuracy, F1 score, and confusion matrix
- Compare model vs. rule-based performance

### 7. Reporting
- Answer all guiding questions from the case study
- Present visual findings, model comparisons, and insights
- Collaboratively compile results into a final presentation deck

## Data
The dataset includes:
- Time-stamped readings of voltage and frequency (every 2 minutes)
- Room and hospital metadata
- Known power configurations
- Rule-based estimated power source (used as reference labels)

## Deliverables
- Individual notebooks with EDA, modeling, and results
- Summary report addressing the case study questions
- Presentation deck for final review

---
For full case description, see: `documents/Data Science Case Study 3.pdf`

