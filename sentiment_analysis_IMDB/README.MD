# Sentiment analysis of movie reviews 

Film Junky Union, a cutting-edge new community for fans of classic movies, is developing a system for filtering and categorizing movie reviews. Your goal is to train a model to detect negative reviews automatically. To achieve this, you'll use a dataset of IMDB movie reviews with tagging to build a model that classifies reviews as positive and negative. This must reach an F1 value of at least 0.85.
project instructions

## Tasks
1. Load the data.
2. Preprocess the data, if necessary.
3. Perform an exploratory data analysis and make your conclusion about class imbalance.
4. Performs data preprocessing for modeling.
5. Train at least three different models for the training data set.
6. Test the models for the test data set.
7. Write some reviews and rate them with all the models.
8. Look for the differences between the test results of the models in the previous two points. Try to explain them.
9. Show your findings.

## Data description

Data were taken from Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

The selected fields are described here:

* `review`: the text of the review
* `pos`: the target, '0' for negative and '1' for positive
* `ds_part`: 'training'/'test' for the training/test part of the dataset, respectively

There are other fields in the dataset, you can explore them if you want.