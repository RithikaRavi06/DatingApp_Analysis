# DatingApp_Analysis

## Overview
This project analyzes user engagement patterns on dating apps by examining how demographic and preference-related factors influence matches, conversations, and ghosting behavior. The goal of this project is to better understand modern online dating interactions and identify patterns that can improve user experience and platform design.

This project was completed as part of DS2500 at Northeastern University.

## Research Questions
This project explores the following questions:

- Do different age groups communicate differently?
- What is the gender breakdown of users?
- Does education level influence ghosting behavior?
- Do men and women receive different numbers of matches?
- Can we predict which users will receive higher engagement using machine learning?


## Dataset
The dataset used is an anonymized European Dating App Behavior dataset containing:

- 395 user profiles
- 16 behavioral and demographic features
- Aggregated Tinder interaction data

## Key Variables
- Number of matches
- Number of conversations
- Average conversation length
- Ghosting rate after first message
- Age
- Gender
- Education level
- Age preference filters
- Country

### Data Cleaning & Preprocessing
- Standardized column naming conventions
- Removed statistical outliers using Z-score filtering
- Engineered new features, including:
  - Ghosting rate
  - Age filter range
  - Conversation success indicators

### Exploratory Data Analysis
Visualization techniques used:
- Histograms
- Boxplots
- Bar charts
- Pie charts

### Machine Learning Model
- Random Forest Classifier
- Predicts whether a user becomes a high-match user
- Used ethical modeling practices by avoiding post-interaction leakage features

### Gender Differences
- Women received approximately 2x the number of matches as men
- Men made up the majority of users, but had lower engagement outcomes

### Education & Communication
- Higher education levels correlated with lower ghosting rates
- Suggests communication expectations may influence early conversation success

### Age Patterns
- Most users fell between the ages of 19 and 35
- Age alone was not a strong predictor of engagement

### Preference Behavior
- Wider age filters increased match likelihood
- Suggests openness improves matching success

## Machine Learning Results
- Realistic model accuracy: 67.6%
- Top predictive features:
  - Age
  - Age filter maximum
  - Age filter range
  - Age filter minimum

Models using post-interaction data reached higher accuracy but demonstrated data leakage.

## Ethical Considerations
- The dataset was anonymized to protect user identity
- Analysis avoided sensitive demographic bias in predictive modeling
- Recognized dataset limitations, including:
  - Geographic bias (European users only)
  - Lack of qualitative message content
  - Limited sample size

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook
