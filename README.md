# 🎯 Predictive Analytics Projects

This repository contains two major data analytics projects focused on real-world business challenges: predicting movie success and analyzing employee attrition using machine learning and data visualization techniques.

---
# 📁 Project 1:🎬 Movie Success Prediction & Sentiment Analysis

This project aims to **predict movie box office success** using IMDB/Kaggle data and perform **sentiment analysis** on user reviews to understand viewer perception by genre.

### 🔍 Objectives

- Scrape or import IMDB movie data with box office and ratings.
- Use **VADER (NLTK)** to analyze sentiment from user reviews.
- Build a **regression model** to predict box office performance.
- Visualize **genre-wise sentiment trends**.

## 📊 Data Sources

- [IMDB](https://www.imdb.com/)
- [Kaggle Movie Datasets](https://www.kaggle.com/)

The project assumes datasets include:
- Movie metadata (name, genre, budget, box office, rating)
- Viewer/user reviews

### 🧰 Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK (VADER Sentiment Analyzer)
- Matplotlib, Seaborn
- Jupyter Notebook


### 📈 Deliverables

 ## Python Jupyter Notebook
  [Uploading Movie_Success_Prediction_&_Sentiment Analysis.ipynb…]()

 ## Sentiment analysis plots
  The following visualizations were created to understand how users feel about movies across genres using VADER Sentiment Analysis:

-Genre-wise Sentiment Distribution: Bar plots showing average compound scores by genre.

-Sentiment vs. IMDB Rating: Scatter plots correlating sentiment with official IMDB ratings.

-Sentiment Wordclouds: Frequently used words in positive vs. negative reviews.

-Review Sentiment Histogram: Distribution of compound scores for all reviews.

![Screenshot 2025-05-16 213302](https://github.com/user-attachments/assets/41546dd4-4add-46ed-a795-95cc93cbd574)

![Screenshot 2025-05-16 213313](https://github.com/user-attachments/assets/4ab6edb9-373e-413a-bb7d-dcbe87fd12d4)

 ## Predictive model summary
  A regression model was developed to predict box office success using factors such as:
  Budget
  IMDB rating
  Genre (one-hot encoded)
  Average sentiment score

✅ Model Details:

Algorithm: Linear Regression (also tested Random Forest)

Target: Box Office Revenue

Evaluation Metrics: R² Score: 0.78 (indicates strong fit)

RMSE: $4.2M (approx.)

🔍 Insights:

Budget and sentiment score were strong predictors.

Some genres (e.g., Action, Comedy) showed consistent under- or over-performance relative to sentiment.

Detailed model metrics and interpretation are in:
[model_summary.txt](https://github.com/user-attachments/files/20256440/model_summary.txt)

---

## 🧠 Key Components

### 1. **Data Collection**
- Imported IMDB/Kaggle datasets using `pandas`
- Cleaned and preprocessed using `pandas` and `numpy`

### 2. **Sentiment Analysis**
- Applied **VADER SentimentIntensityAnalyzer** from NLTK
- Extracted compound scores from reviews
- Analyzed sentiment trends across genres

### 3. **Box Office Prediction**
- Created regression models using `scikit-learn`
- Features: Genre, budget, sentiment score, etc.
- Model evaluation: R² Score, RMSE

### 4. **Visualization**
- Plotted sentiment polarity by genre
- Correlation heatmaps
- Predicted vs actual box office revenue

## 📌 Results

- **Regression Model Summary**: Found strong correlations between budget, sentiment scores, and box office success.
- **Sentiment Trends**: Animated, Drama, and Sci-Fi genres showed the highest viewer positivity.


---
# 📁 Project 2: 🧑‍💼 Employee Attrition Analysis & Prediction

This project uses **HR analytics** to understand key factors driving employee resignations and build a predictive model to reduce future attrition.

### 🔍 Objectives

- Perform EDA on HR data (department-wise attrition, salary bands, promotions, etc.)
- Build a classification model (Logistic Regression or Decision Tree)
- Visualize attrition factors with **Power BI**
- Use **SHAP** values to interpret model predictions

### 📊 Data Source
The HR dataset was sourced from a Kaggle dataset titled "HR Analytics: Employee Attrition"
[HR_Analytics.csv](https://github.com/user-attachments/files/20256574/HR_Analytics.csv)

It includes over 1,400 employee records with features like:

-JobRole, MonthlyIncome, OverTime, YearsAtCompany

-PerformanceRating, PromotionLast5Years, JobSatisfaction

-Attrition (Target variable: Yes/No)

The dataset was cleaned, encoded, and balanced for training the classification model.


### 🧰 Tools & Technologies

- Python (Pandas, Seaborn)
- Scikit-learn
- SHAP
- Power BI
- Jupyter Notebook


### 📈 Deliverables

- Power BI dashboard (.pbix)
- Model accuracy report with confusion matrix
  ![confusion_matrix](https://github.com/user-attachments/assets/931b41a3-7a8f-4d22-9a79-fed11f5ab0da)

- PDF report of attrition prevention suggestions
  [attrition_suggestions.pdf](https://github.com/user-attachments/files/20256509/attrition_suggestions.pdf)


---
### 🧠 Results
✅ Classification Model Performance:
Model Used: Decision Tree Classifier (Logistic Regression also tested)

Accuracy: 84%

Precision: 81%

Recall: 79%

F1 Score: 80%
