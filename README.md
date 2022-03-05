# Fake News Detection
## Context
A king of yellow journalism, fake news is false information and hoaxes spread through social media and other online media to achieve a political agenda. We will use Python to build a model that can accurately detect whether a piece of news is real or fake. We’ll build a TfidfVectorizer and evalualte moulitple models' performance in classifying news as either “Real” or “Fake”. 
## Dataset
Fake News dataset from Kaggle Competition (https://www.kaggle.com/c/fake-news/data)
## Objective
Evaluate performance between Passive Aggressive Classifer, Multinomial Naive Bayes, and Logistic Regression Models
## Steps
* Data processing of Fake News datasets
* Prepare Porter Stemming on News datasets
* Converting the textual data to numerical data using TfIdf vectorizer
* Run training for Passive Aggressive Classifer, Multinomial Naive Bayes, and Logistic Regression Models
* Compare performance (Accuracy, F1, etc.) and time
## Results
* The Passive Aggressive Model outperformed both the Multinomial Naive Bayes and Logistic Regression Models
* In decreasing **acurracy**:
    * Passive Aggressive: 99%
    * Logistic Regression: 98%
    * Multinomial Naive Bayes: 95%
## References
* https://www.nltk.org/
* https://www.kaggle.com/c/fake-news/overview
* https://www.geeksforgeeks.org/passive-aggressive-classifiers/#:~:text=Passive%2DAggressive%20algorithms%20are%20called,make%20changes%20to%20the%20model.