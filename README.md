# ReviewSense – Extracting Insights from Customer Feedback

## Milestone 1 & Milestone 2 README

---

## Project Overview

**ReviewSense** is a customer feedback analytics project designed to transform raw customer reviews into meaningful business insights.
The project consists of two milestones:

* **Milestone 1:** Data Ingestion & Text Cleaning
* **Milestone 2:** Sentiment Analysis & Insight Generation

Together, these steps create a complete pipeline that prepares raw feedback, analyzes customer sentiment, and generates analytical outputs for further decision-making and visualization.

---

## Milestone 1 – Data Ingestion & Text Cleaning

### Objective

Collect raw customer feedback data, clean textual noise (URLs, punctuation, numbers, stopwords, extra spaces), and produce a standardized dataset ready for analysis.

### Key Features

* Reads customer feedback from Excel file
* Cleans text using preprocessing techniques
* Removes:

  * URLs
  * Numbers
  * Punctuation
  * Stopwords
  * Extra spaces
* Generates cleaned feedback column
* Saves processed dataset for further analysis

### Input

`ReviewSense_Customer_Feedback_5000.xlsx`

### Output

`Milestone1_Cleaned_Feedback.csv`

### Technologies Used

* Python
* pandas
* re (Regular Expressions)
* string

---

## Milestone 2 – Sentiment Analysis & Visualization

### Objective

Analyze cleaned feedback text using Natural Language Processing to determine sentiment polarity (positive, negative, neutral), generate confidence scores, and visualize overall sentiment distribution.

### Key Features

* Sentiment classification using polarity scoring
* Labels feedback as:

  * Positive
  * Negative
  * Neutral
* Generates confidence score (range −1 to +1)
* Saves updated dataset with sentiment results
* Creates sentiment distribution bar chart

### Input

`Milestone1_Cleaned_Feedback.csv`

### Outputs

* `Milestone2_Sentiment_Results_new.csv`
* `sentiment_bar_chart.png`

### Technologies Used

* Python
* pandas
* TextBlob
* matplotlib

---

## Project Workflow

1. Load raw customer feedback dataset.
2. Clean the feedback text (Milestone 1).
3. Save cleaned dataset.
4. Perform sentiment analysis on cleaned text (Milestone 2).
5. Generate sentiment labels and confidence scores.
6. Save results and create visualization.

---

## Installation

Install required libraries:

```
pip install pandas openpyxl textblob matplotlib
```

---

## How to Run

### Step 1 – Run Data Cleaning

```
python milestone1.py
```

### Step 2 – Run Sentiment Analysis

```
python milestone2.py
```

---

## Expected Results

* Cleaned feedback dataset ready for analysis
* Sentiment-labeled dataset
* Visual chart showing customer sentiment distribution

---

## Future Enhancements

* Topic classification of feedback
* Dashboard visualization using Streamlit
* Machine learning–based predictive sentiment modeling
* Product-wise and region-wise feedback analytics

---

