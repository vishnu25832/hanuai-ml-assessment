# HanuAi Machine Learning Assessment

## Overview

This repository contains the deliverables for **Task 1 and Task 2** of the HanuAi Machine Learning Assessment.

HanuAi focuses on AI-driven solutions for engineering quality and safety, particularly in road and infrastructure maintenance. This assessment focuses on data analytics, text mining, sentiment analysis, and transforming raw data into actionable business insights.

The objective is to demonstrate an understanding of data and analytical tools, identify meaningful patterns, and communicate findings and recommendations to stakeholders.

## Repository Structure

```text
HanuAi_ML_Assessment/
├── Task1/
│   └── Web Scraping and Sentiment Analysis deliverables
├── Task2/
│   └── Advanced EDA and Text Mining deliverables
├── Readme.md
└── .gitignore
```

## Task 1: Web Scraping and Sentiment Analysis

### Objective

Develop a Python-based solution to collect publicly accessible product reviews from Best Buy Canada and perform sentiment analysis to identify customer opinions, satisfaction drivers, and areas for improvement.

Website: https://www.bestbuy.ca/en-ca

### Key Requirements

- Select a product with at least 50 reviews.
- Use a suitable Python web scraping library, such as Selenium or Beautiful Soup.
- Handle pagination and review filters, including Most Helpful, Newest, Highest Rating, Lowest Rating, and Most Relevant, where supported by the website.
- Extract review information, including:
  - Primary key or review identifier
  - Review title
  - Review text
  - Review date in `YYYY-MM-DD` format
  - Rating out of 5
  - Source
  - Reviewer name, where publicly available
- Apply an appropriate sentiment analysis technique or model to categorize review text.
- Document responsible scraping practices and approaches to handling errors, rate limits, and anti-scraping restrictions.
- Summarize customer satisfaction and dissatisfaction drivers and provide actionable business recommendations.

### Expected Deliverables

1. Jupyter Notebook (`.ipynb`) containing the scraping and sentiment analysis implementation, with code comments and explanations.
2. CSV or Excel file containing the extracted review fields and sentiment classifications.
3. Stakeholder report documenting scraping challenges, analytical findings, and recommendations.

### Responsible Scraping

The implementation should respect the website's terms, applicable policies, and access restrictions. It should use reasonable request rates, retries with backoff, and appropriate error handling. CAPTCHA challenges and access restrictions should not be bypassed without authorization.

## Task 2: Advanced Exploratory Data Analysis and Text Mining

### Objective

Perform comprehensive exploratory data analysis, extract structured information from unstructured text, identify recurring issue categories, and generate actionable insights from the provided dataset.

### Exploratory Data Analysis

- Examine dataset size, column names, data types, and distributions.
- Identify and handle missing values, duplicate records, and data inconsistencies where appropriate.
- Identify important columns for stakeholder analysis.
- Produce descriptive statistics and relevant visualizations.
- Document data preparation decisions and significant observations.

### Text Mining and NLP

- Identify free-text columns in the source dataset.
- Apply suitable text-mining or NLP techniques to extract meaningful tags and entities.
- Convert relevant unstructured information into structured fields.
- Group extracted entities into meaningful issue categories, such as component failures or electrical issues, where supported by the data.
- Document the methods used and any limitations in interpreting the extracted information.

### Clustering and Topic Analysis

- Apply suitable clustering or topic-modelling techniques to group recurring failure modes, issues, or complaints.
- Evaluate clustering results using appropriate validation metrics.
- Investigate recurring patterns and potential root causes without treating exploratory groupings as confirmed causal relationships.
- Identify significant trends and frequently reported issues.

### Stakeholder Insights and Business Value

Translate analytical findings into recommendations that could help stakeholders:

- Identify frequently occurring failures or complaints.
- Prioritize areas for product quality and performance improvement.
- Investigate recurring issues and potential root causes.
- Improve maintenance planning and operational decision-making.
- Establish opportunities for further analysis and monitoring.

### Expected Deliverables

1. Jupyter Notebook (`.ipynb`) containing the EDA, text mining, and analytical implementation, with code comments and explanations.
2. CSV or Excel file containing extracted tags and other relevant structured outputs.
3. Stakeholder report covering the data, analytical findings, potential customer value, actionable recommendations, business impact, key learnings, and further improvements.

## Technologies and Tools

Depending on the implementation, the assessment may use:

- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Selenium or Beautiful Soup
- NLP and sentiment analysis techniques
- Clustering or topic-modelling methods
- CSV and Excel for structured outputs

Refer to the notebooks and supporting files in each task folder for the specific tools and methods used.

## How to Review the Submission

1. Open `Task1/` to review the web scraping, sentiment analysis, generated data files, and stakeholder report, if included.
2. Open `Task2/` to review the EDA and text-mining notebook, processed data, extracted outputs, visualizations, and stakeholder report.
3. Review the analysis notebooks and reports together to understand the methods, findings, limitations, and recommendations.

Use the Python environment and dependencies required by the relevant notebooks.

## Submission and Reproducibility Notes

- Task 1 and Task 2 are organized into separate folders within one repository.
- Required notebooks, datasets, generated outputs, visualizations, and reports should be included where applicable.
- Generated results should be interpreted in the context of the source data and the limitations of the analytical methods.
- Virtual environments, cache folders, temporary files, credentials, and secrets should not be committed.
- Any external data source should be used in accordance with its applicable terms and access policies.

---

**Assessment:** HanuAi Machine Learning Assessment  
**Tasks:** Task 1 — Web Scraping and Sentiment Analysis; Task 2 — Advanced EDA and Text Mining