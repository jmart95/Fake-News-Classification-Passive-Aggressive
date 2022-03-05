# Fake News Detection
## Context
The Passive-Aggressive classifier takes in one piece at a time, adjusting the weights of its model based on each entry's results. If the prediction is correct, the model is not changed: it is "passive." If the prediction is incorrect, it adjusts the weights of the model until the prediction becomes correct. PA algorithms are ideal for classifying massive streams of data. We’ll build a TfidfVectorizer and evalualte a couple models' performance against the PA model classifying news as either “Real” or “Fake”. 
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
* https://iopscience.iop.org/article/10.1088/1742-6596/1693/1/012158/pdf