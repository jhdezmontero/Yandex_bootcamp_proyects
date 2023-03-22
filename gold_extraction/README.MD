# Project description
Prepare a prototype of a machine learning model for **Zyfra**. The company develops efficiency solutions for heavy industry.
The model must predict the amount of gold extracted. You have the extraction and purification data.
The model will help to optimize production and eliminate unprofitable parameters.
You will have to:

1. Prepare the data;
2. Perform data analysis;
3. Develop a model and train it.

## Data description
The data is stored in three files:

* gold_recovery_train.csv
* gold_recovery_test.csv 
* gold_recovery_full.csv 

The data is indexed with the date and time of acquisition (date). Parameters close in time are usually similar.
Some parameters are not available because they were measured or calculated much later. Therefore, some of the features that are present in the training set may be absent in the test set. The test set also contains no targets.
The source dataset contains the training and test sets with all features.
You have at your disposal the raw data that was only downloaded from the data warehouse. Before building the model, check that the data is correct.

## Model training

1. Write a function to calculate the final value of sMAPE.
2. Train different models. Evaluate them by applying cross validation. Choose the best model and test it using the test sample. It facilitates the results.

Use these formulas for evaluation metrics:

$$sMAPE = \frac{1}{N} \sum_{i=1}^{N} \frac{|y_{i}-\hat{y}_i|}{(|y_{i}|+|\hat{y}_{i}|)/2} · 100$$

$$sMAPE_final = 25% · sMAPE(rougher) + 75% · sMAPE(final)$$