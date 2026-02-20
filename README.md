# ReviewSense – Extracting Insights from Customer Feedback

## Complete README (Milestone 1, 2 & 3)

---

## Project Overview

**ReviewSense** is a customer feedback analytics pipeline that converts raw customer reviews into meaningful business insights.
The project is developed across three milestones that progressively transform unstructured feedback into analytical intelligence.

* **Milestone 1:** Data Ingestion & Text Cleaning
* **Milestone 2:** Sentiment Analysis & Visualization
* **Milestone 3:** Keyword Insight Extraction

Together, these stages help identify customer sentiment, common discussion topics, and actionable insights.

---

## Milestone 1 – Data Ingestion & Text Cleaning

### Objective

Prepare raw customer feedback for analysis by cleaning noisy textual data.

### Key Features

* Reads feedback from Excel or CSV
* Removes URLs, numbers, punctuation, stopwords, and extra spaces
* Generates standardized cleaned text
* Handles missing files gracefully
* Produces analysis-ready dataset

### Input

`ReviewSense_Customer_Feedback_5000.xlsx`

### Output

`Milestone1_Cleaned_Feedback.csv`

### Technologies

* Python
* pandas
* re (Regular Expressions)
* string

---

## Milestone 2 – Sentiment Analysis & Visualization

### Objective

Determine customer sentiment using Natural Language Processing and generate visual summaries.

### Key Features

* Uses TextBlob polarity scoring
* Labels feedback as:

  * Positive
  * Negative
  * Neutral
* Generates confidence score (−1 to +1)
* Saves sentiment results
* Creates sentiment distribution bar chart

### Input

`Milestone1_Cleaned_Feedback.csv`

### Outputs

* `Milestone2_Sentiment_Results_new.csv`
* `sentiment_bar_chart.png`

### Technologies

* Python
* pandas
* TextBlob
* matplotlib

---

## Milestone 3 – Keyword Insight Extraction

### Objective

Identify the most frequently discussed topics in customer feedback using keyword frequency analysis.

### Key Features

* Extracts keywords from cleaned feedback
* Removes special characters and noise
* Counts keyword frequency using Counter
* Generates ranked keyword insights
* Helps identify major customer concerns and themes

### Input

`Milestone2_Sentiment_Results_new.csv`

### Output

`Milestone3_Keyword_Insights.csv`

### Technologies

* Python
* pandas
* collections.Counter
* re

---

## Project Workflow

1. Collect raw customer feedback.
2. Clean and standardize text (Milestone 1).
3. Analyze sentiment and generate visualization (Milestone 2).
4. Extract most frequent keywords for topic insights (Milestone 3).
5. Produce datasets ready for dashboards, reporting, and future modeling.

---

## Installation

Install required libraries:

```
pip install pandas openpyxl textblob matplotlib
```

---

## How to Run

### Step 1 – Text Cleaning

```
python milestone1.py
```

### Step 2 – Sentiment Analysis

```
python milestone2.py
```

### Step 3 – Keyword Insights

```
python milestone3.py
```

---

## Final Outputs Summary

* Cleaned feedback dataset
* Sentiment-labeled dataset with confidence scores
* Sentiment visualization chart
* Keyword frequency insights dataset

---

## Typical Use Cases

* Customer satisfaction monitoring
* Product improvement analysis
* Support quality evaluation
* Trend detection
* Dashboard creation
* Foundation for machine learning models

---

## Future Enhancements

* Topic classification dashboard using Streamlit
* Product-wise sentiment analysis
* Trend analysis over time
* Machine learning–based sentiment prediction
* Real-time feedback monitoring

