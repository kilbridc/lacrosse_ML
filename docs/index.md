# Lacrosse ML Project

## Introduction
This project explores the key factors that contribute to the success of NCAA Division I Men’s Lacrosse teams. Using game data and tracked performance metrics, I applied multiple machine learning models to identify which aspects of gameplay are most strongly associated with winning outcomes.

Rather than trying to perfectly predict winners, the goal was to gain insight into the **statistics most closely tied to team success**, such as possession metrics, scoring efficiency, and riding/clearing effectiveness. These findings help highlight the strategic elements of the game that matter most.

As lacrosse continues to grow rapidly in popularity, **recent rule changes** — including the introduction of a shot clock, adjustments to faceoff rules, and the rise of the aggressive 10 Man Ride — have significantly influenced how the game is played. This project also considers how these changes impact strategy and statistical trends.

## 📊 Results Summary

I evaluated model performance using accuracy and F1-score. **Logistic Regression with L1 regularization** performed best, suggesting a mostly linear relationship in the data and that only a few key features drive team success.

### 🔎 Model Summaries

- **Logistic Regression**  
  Best overall performance with L1 regularization. Highlighted a small number of impactful features. RPI, Turnovers/Game, and Assists/Game stood out. L1 regularization outperformed L2, suggesting feature sparsity is important.

- **Random Forest**  
  Good performance and interpretability via feature importance. Key features included RPI, Average Margin, and Goals/Game. Showed slightly more noise than logistic regression.

- **XGBoost**  
  Feature importance measured using gain. Top features included RPI, Average Margin, and Saves/Game. Offered additional insight into subtle non-linear relationships.

### 🔑 Key Features Across Models

- **RPI** was the most consistent predictor pre- and post-2020.
- **Turnovers per Game** had a strong negative correlation with winning.
- **Average Margin** and **Faceoff Percentage** also ranked highly.
- **Saves per Game** showed a surprising negative correlation, likely due to more shots allowed.

### ⚙️ Impact of Rule Changes

Post-2020, **RPI became even more important**, while **Assists per Game** dropped in significance — likely due to the increased pace of play reducing setup time for assisted shots. **Clearing stats** had low importance overall.

## Links

[Link to the GitHub Repository](https://github.com/kilbridc/lacrosse_ML)

[Open The Notebook in Google Colab](https://colab.research.google.com/github/kilbridc/lacrosse_ML/blob/main/Final_Notebook.ipynb)

[Watch the video report about this project](https://youtu.be/dWswCVBtA3E)

[Download the report (PDF)](https://raw.githubusercontent.com/kilbridc/lacrosse_ML/main/Reports/Executive_Report.pdf)

