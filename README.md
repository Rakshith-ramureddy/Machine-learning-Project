# Machine-learning-Project


**Overview:**
This report is divided into two main parts: the analysis and prediction of transport mode preferences of employees at ABC Consulting, and a text mining exercise on Shark Tank episodes data.

**Part 1: Machine Learning Models**

**Objective:** 
To predict the preferred mode of transport for employees of ABC Consulting based on parameters such as age, salary, work experience, etc.

**Data Summary:**
- Dataset: Transport.csv
- Columns: Age, Gender, Engineer, MBA, Work Experience, Salary, Distance, License, Transport Mode
- Total Records: 444
- No missing or null values identified.

**Univariate and Bivariate Analysis:**
- Numerical columns (Age, Work Experience, Salary, Distance) exhibit right skewness and contain outliers.
- Correlation analysis indicates Age and Work Experience, Age and Salary, and Work Experience and Salary are highly correlated.

**Outlier Treatment and Data Scaling:**
- Outliers were identified and treated.
- Min-max scaling was applied to standardize the features due to differing "weights".

**Model Training and Evaluation:**
- Models: Logistic Regression, Linear Discriminant Analysis (LDA), Decision Tree (CART), Naïve Bayes, K-Nearest Neighbors (KNN), Random Forest, Gradient Boosting Classifier.
- Data Split: 70% training, 30% testing.
- Evaluation Metrics: Confusion Matrix, ROC Curve, AUC values.

**Model Performance:**
- Gradient Boosting Classifier achieved the highest performance with an AUC score of 0.98 and accuracy of 92% on training data and 81% on testing data.
- KNN Model was the second best with an AUC score of 0.922.
- Decision Tree (CART) performed the worst.

**Business Insights:**
- Majority prefer public transport.
- Factors influencing transport choice include age, salary, and distance from home to office.
- Employees traveling more than 20 km typically prefer private transport.
- A larger dataset could improve model accuracy.

**Part 2: Text Mining**

**Objective:**
To analyze descriptions of Shark Tank pitches to determine if certain words or themes correlate with securing a deal.

**Data Summary:**
- Dataset includes 495 entrepreneurs' pitches.
- Key columns: Deal (dependent variable) and Description.

**Analysis Steps:**
1. Separate data into two corpora: one for pitches that secured deals and one for those that did not.
2. Remove stop words and identify the top 3 most frequently occurring words in each corpus.
3. Create word clouds for both corpora.

**Findings:**
- Total Characters: Secured Deal Corpus - 64,060; Not Secured Deal Corpus - 47,184.
- Common Words: "make, made, company, product."
- Secured Deal Corpus: Words like "online service, designed, system, offer, free, easy" were prominent.
- Not Secured Deal Corpus: Words like "service, without, people, device, traditional, food, fitness" were prominent.

**Inference:**
- Entrepreneurs pitching "devices" are less likely to secure a deal, but this is not definitive. Other factors such as business model and presentation likely play roles.
- Further detailed analysis is needed for more concrete conclusions.

**Conclusion:**
The report successfully identifies the key factors influencing transport mode preference using machine learning models and provides insights into Shark Tank pitches through text mining, suggesting potential strategies for securing deals based on word usage.
