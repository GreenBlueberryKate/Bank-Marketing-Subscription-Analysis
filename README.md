# Bank-Marketing-Subscription-Analysis
📊 Bank Marketing Subscription Analysis — Interpretable Modeling Project
🧭 Project Overview

This project analyzes customer behavior in a bank marketing campaign with the goal of understanding what drives term deposit subscriptions and how marketing teams can make more informed targeting decisions.

Rather than focusing on complex machine learning, the analysis emphasizes behavioral exploratory data analysis (EDA) and interpretable modeling to produce insights that are transparent and actionable for stakeholders.

The final model is a logistic regression classifier designed to rank customers by subscription likelihood using only information available before a call is made.

🎯 Objectives

Explore behavioral and demographic patterns influencing subscription decisions.

Identify meaningful predictors through structured EDA.

Build an interpretable classification model.

Translate model results into business-oriented insights.

📂 Dataset

Bank Marketing Dataset

Binary classification problem: whether a client subscribes to a term deposit.

Includes demographic attributes, campaign history, and contact information.

Target variable:

y_binary — subscription outcome (yes/no).

🔎 Analytical Approach
1. Behavioral Exploratory Data Analysis

Key steps included:

Creation of an age_band feature to improve interpretability.

Investigation of categorical drivers such as job role, education level, and previous campaign outcome.

Identification of strong behavioral signals, especially prior campaign success (poutcome).

Detection and removal of data leakage (duration variable excluded from modeling).

Main EDA insight:

Historical engagement with previous campaigns shows stronger influence than most demographic characteristics.

2. Feature Engineering

One-hot encoding of categorical variables using get_dummies(drop_first=True).

Focus on interpretable transformations aligned with business understanding.

3. Modeling — Logistic Regression

An interpretable logistic regression model was trained to estimate subscription probability.

Why logistic regression?

Transparent coefficient interpretation.

Alignment with behavioral insights from EDA.

Suitable for probability-based customer ranking.

Key modeling outcome:

poutcome_success emerged as the strongest predictor, reinforcing the importance of past campaign engagement.

📈 Model Interpretation

Instead of optimizing for raw accuracy, the model is treated as a decision-support tool:

Coefficients are interpreted as behavioral signals.

Predictions are used to rank customers by likelihood of subscription.

The approach highlights how targeting strategy and customer history drive outcomes.

💡 Key Business Insights

Past campaign success is the most influential driver of future subscriptions.

Behavioral engagement signals outweigh most static demographic features.

Interpretable models can support marketing prioritization without sacrificing transparency.

🧠 Analytical Mindset

This project prioritizes:

Reasoning over algorithm complexity.

Clear storytelling over purely technical metrics.

Responsible modeling choices (e.g., leakage avoidance).

🚀 Potential Next Steps

Evaluate probability thresholds for targeted outreach strategies.

Compare top-probability customer segments against baseline conversion rates.

Explore interaction effects between demographics and campaign history.

🛠️ Tools & Libraries

Python

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn
