# HanuAi ML Assessment — Task 1: Web Scraping and Sentiment Analysis

## Project Overview

This project focuses on collecting customer reviews for the Logitech H540 USB Headset for PC from Best Buy Canada and performing sentiment analysis to understand customer feedback.

The project uses Python-based browser automation, HTML parsing, data preprocessing, and sentiment classification to organize and analyze customer reviews.

**Product:** Logitech H540 USB Headset for PC  
**Review Source:** [Best Buy Canada](https://www.bestbuy.ca/en-ca/product/logitech-logitech-usb-headset-h540-981-000510/10218414/review)

## Objectives

- Extract customer review information from a product review page.
- Organize review titles, text, dates, ratings, and reviewer names.
- Clean and preprocess the collected data.
- Classify reviews as positive, neutral, or negative.
- Visualize the sentiment distribution.
- Identify preliminary customer feedback trends and business recommendations.

## Technologies Used

- Python
- Selenium
- BeautifulSoup
- Pandas
- NumPy
- VADER Sentiment Analysis
- Matplotlib
- Jupyter Notebook

## Methodology

### 1. Web Scraping

Selenium was used to access the product review page, while BeautifulSoup and HTML inspection were used to identify and parse review information.

The target fields included:

- Primary Key
- Review Title
- Review Text
- Review Date
- Rating out of 5
- Source
- Reviewer Name

### 2. Data Preprocessing

Pandas was used to structure the collected reviews, standardize dates, convert ratings to numeric values, handle missing text fields, remove duplicate records, and generate unique primary keys.

### 3. Sentiment Analysis

VADER was used to calculate compound sentiment scores and classify reviews into three categories:

- **Positive:** Compound score ≥ 0.05
- **Neutral:** Compound score > -0.05 and < 0.05
- **Negative:** Compound score ≤ -0.05

### 4. Visualization

Matplotlib was used to generate a bar chart representing the sentiment distribution of the collected review sample.

## Results

The initial accessible page yielded 10 review records.

| Sentiment | Reviews | Percentage |
|---|---:|---:|
| Positive | 8 | 80% |
| Neutral | 0 | 0% |
| Negative | 2 | 20% |
| **Total** | **10** | **100%** |

These results apply only to the collected sample and should not be interpreted as representative of all customers.

## Business Insights

- Most reviews in the sample were classified as positive by VADER.
- Negative reviews should be examined individually to identify possible product concerns.
- Combining sentiment scores with star ratings may help identify inconsistencies in customer feedback.
- A larger, representative dataset is needed before drawing reliable conclusions about overall customer satisfaction.

## Challenges and Limitations

During subsequent scraping attempts, Selenium received an **Access Denied** response from the product review page. This prevented the collection of additional reviews using the existing approach.

The notebook includes debugging checks and preserves the initially collected records. Further collection should use a method authorized for the assignment.

**Important:** The assignment specifies a minimum of 50 reviews. Only 10 reviews were successfully collected, so this requirement remains outstanding. The sentiment analysis is preliminary and based on this limited sample.

## Project Files

| File | Description |
|---|---|
| `Task1_Scraper.ipynb` | Notebook containing the setup, scraping, debugging, preprocessing, and analysis code |
| `bestbuy_reviews_backup.csv` | Backup of the initially collected reviews |
| `task1_reviews_sentiment.csv` | Processed review data with sentiment scores and labels |
| `bestbuy_sentiment_distribution.png` | Sentiment distribution chart |

*Verify that these files exist in the repository before relying on this file list.*

## Conclusion

This project demonstrates a workflow for browser automation, review extraction, data preprocessing, sentiment analysis, and visualization using Python.

The sentiment-analysis pipeline was tested on 10 collected reviews. However, the minimum 50-review requirement remains incomplete because subsequent collection attempts encountered an access restriction. Additional authorized data collection is needed to complete that requirement.

## Author

Prepared as part of the HanuAi Machine Learning Assessment.
