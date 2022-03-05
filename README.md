# Fake-News-Detection
## Context
A king of yellow journalism, fake news is false information and hoaxes spread through social media and other online media to achieve a political agenda. In this data science project idea, we will use Python to build a model that can accurately detect whether a piece of news is real or fake. We’ll build a TfidfVectorizer and use a PassiveAggressiveClassifier to classify news into “Real” and “Fake”. We’ll be using a dataset of shape 7796×4 and execute everything in Jupyter Lab.
## Dataset
Simulated credit card transaction data from the research collaboration between Worldline and Machine Learning Group (https://github.com/Fraud-Detection-Handbook/simulated-data-transformed)
## Objective
Evaluate performance of AutoXGB against the standard XGBoost + RandomizedSearchCV setup
## Steps
* Data processing of credit card transaction dataset, with special focus on handling class imbalance with SMOTE and Random Undersampling
Select appropriate performance metric for binary classification task i.e. Average Precision
Run training for baseline model: XGBoost with RandomizedSearchCV
Run training for AutoXGB
Compare performance and speed
## Results
AutoXGB delivered a slightly higher Average Precision score of 0.782 as compared to the baseline score of 0.776.
The time taken for AutoXGB training is approximately 30% shorter, taking just 9 minutes as compared to the baseline of 13 minutes.
Another key advantage of AutoXGB is that we are only one command line away from serving the model as a FastAPI endpoint. This setup reduces the time to model deployment, which is a critical factor beyond training time.
While the performance metrics give AutoXGB an edge, one of its most significant issues is the loss of granular control in the parameter settings e.g. unable to set eval_metric for XGBClassifier, unable to set specific validation sets for cross-validation
At the end of the day, while solutions like AutoXGB do well in simplifying (and possibly improving) XGBoost implementation, data scientists need to understand its limitations by knowing what goes on under the hood.
## References
* https://www.nltk.org/
* https://www.kaggle.com/c/fake-news/overview