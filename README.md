# 📊 ReviewSense – Extracting Insights from Customer Feedback

## 🚀 Project Overview

**ReviewSense** is a complete customer feedback analytics pipeline that transforms raw customer reviews into actionable business insights.

The project is implemented in four milestones:

1. Data Cleaning & Preparation
2. Sentiment Analysis
3. Keyword Extraction
4. Interactive Dashboard Visualization

The final output is an interactive business intelligence dashboard built using Streamlit.

---

# 🧩 Project Architecture

Raw Feedback
→ Cleaning & Preprocessing
→ Sentiment Classification
→ Keyword Extraction
→ Interactive Dashboard
→ Business Insights

---

# 📌 Milestone 1 – Data Cleaning & Preprocessing

## 🎯 Objective

Clean raw customer feedback and prepare it for analysis.

## ⚙️ Tasks Performed

* Removed special characters
* Converted text to lowercase
* Removed extra spaces
* Standardized formatting
* Generated cleaned feedback column

## 📂 Input

Raw customer feedback dataset (CSV)

## 📤 Output

`Milestone1_cleaned_feedback.csv`

## 🛠 Technologies Used

* Python
* pandas
* Regular Expressions (re)

---

# 📌 Milestone 2 – Sentiment Analysis

## 🎯 Objective

Classify customer feedback into:

* Positive
* Negative
* Neutral

## ⚙️ Tasks Performed

* Applied TextBlob polarity scoring
* Assigned sentiment label based on polarity
* Stored confidence score
* Generated sentiment distribution
* Created sentiment bar chart

## 📂 Input

`Milestone1_cleaned_feedback.csv`

## 📤 Output

`Milestone2_Sentiment_Results_new.csv`
`sentiment_bar_chart.png`

## 🛠 Technologies Used

* Python
* pandas
* TextBlob
* matplotlib

## 📊 Output Columns

* clean_feedback
* sentiment
* confidence_score

---

# 📌 Milestone 3 – Keyword Extraction

## 🎯 Objective

Identify most frequently occurring keywords in customer feedback.

## ⚙️ Tasks Performed

* Converted text to lowercase
* Removed special characters
* Tokenized words
* Counted word frequency using Counter
* Sorted keywords by frequency

## 📂 Input

`Milestone2_Sentiment_Results_new.csv`

## 📤 Output

`Milestone3_Keyword_Insights.csv`

## 🛠 Technologies Used

* Python
* pandas
* collections.Counter
* re (regex)

## 📊 Output Columns

* keyword
* frequency

---

# 📌 Milestone 4 – Interactive Dashboard

## 🎯 Objective

Transform sentiment and keyword analysis into an interactive dashboard.

## ⚙️ Features Implemented

### 🔍 Sidebar Filters

* Sentiment filter (Positive, Negative, Neutral)
* Product filter
* Date range filter

### 📊 KPI Metrics

* Total Reviews
* Positive %
* Negative %
* Neutral %

### 📈 Visualizations

* Sentiment distribution bar chart
* Product-wise sentiment table
* Product sentiment heatmap
* Monthly sentiment trend graph
* Top keyword frequency chart
* Word cloud
* Confidence score histogram

### 📥 Export Options

* Download filtered reviews (CSV)
* Download keyword list (CSV)

---

## 📂 Inputs

* `Milestone2_Sentiment_Results_new.csv`
* `Milestone3_Keyword_Insights.csv`

## 📤 Outputs

* Interactive Streamlit dashboard
* Exportable CSV files:

  * ReviewSense_Filtered_Reviews.csv
  * ReviewSense_Keywords.csv

---

# 🛠 Technology Stack

* Python
* pandas
* TextBlob
* matplotlib
* seaborn
* WordCloud
* Streamlit

---

# ▶️ Installation Guide

### Step 1 – Install Dependencies

```bash
pip install pandas textblob matplotlib seaborn wordcloud streamlit
```

---

### Step 2 – Run Sentiment Analysis

```bash
python milestone2.py
```

---

### Step 3 – Run Keyword Extraction

```bash
python milestone3.py
```

---

### Step 4 – Launch Dashboard

```bash
python -m streamlit run milestone4.py
```

---

# 📈 Business Value

ReviewSense enables organizations to:

* Monitor customer satisfaction
* Compare product performance
* Identify recurring issues
* Detect trends over time
* Make data-driven decisions
* Export insights for reporting

---

# 🧠 Key Learning Outcomes

* Text preprocessing
* Sentiment analysis using NLP
* Keyword extraction
* Data visualization
* Dashboard development
* Business intelligence reporting

---

# 🏁 Conclusion

ReviewSense successfully transforms raw customer feedback into structured insights using sentiment analysis, keyword extraction, and interactive visualization.

The project demonstrates a complete end-to-end data analytics pipeline suitable for real-world business applications.

