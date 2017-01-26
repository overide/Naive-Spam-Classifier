# Naive-Spam-Classifier
This is a simple Spam classifier, which will classify email either spam or not. It uses Naive Bayes Algorithm for classification, which is implemented from scratch ;)

## Project Structure
Keep a folder named **dataset** where your training data resides.Directory structure is like this-
```
dataset
|
|-- spam
|-- not_spam
```

**spam** folder contain spam emails data and **not_spam** folder contain non spam email data<br>
Spam Email dataset - https://spamassassin.apache.org/publiccorpus/20021010_spam.tar.bz2<br>
Non Spam Email dataset - https://spamassassin.apache.org/publiccorpus/20021010_easy_ham.tar.bz2

## Usage
**NaiveBayesClassifier** class have method **classify** which will take any message and output it's probability of being spam
``` python
>>>classifier = NaiveBayesClassifier()
>>>classifier.train(train_data)
>>>classifier.classify("Get free laptops now!")
>>>0.99453546456
```
Training dataset take a list of tuple (subject, is_spam). Subject is subject of email and is_spam is boolean value indication whether email is spam or not
