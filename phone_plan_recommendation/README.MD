# Project Description

The **Megaline** mobile company is not satisfied to see that many of its customers use legacy plans. They want to develop a model that can analyze the customer behavior and recommend one of Megaline's new plans: Smart or Ultra.

For this classification task you must create a model that chooses the correct plan.

To help you train your model, you will use user behavior data of the course on Statistical data analysis. As you already did the step of processing the data, you can jump right into creating the model.

Develop a model as accurately as possible. In this project, the threshold of
accuracy is **0.75**. Use the dataset to check the accuracy.


## Instructions

1. Open and examine the data file. Address to the file: datasets/users_behavior_upd.csv
2. Segment the source data into a training set, a validation set, and test one.
3. Investigate the quality of different models by changing the hyperparameters. Briefly describe the study findings.
4. Check the quality of the model using the test set.
5. Bonus Task: Test the sanity of the model. 

## Data description

Each observation in the dataset contains information on the monthly behavior about a user. The information given is as follows:

* `сalls` — number of calls
* `minutes` — total duration of the call in minutes
* `messages` —number of text messages
* `messages` —number of text messages
* `mb_used` — Internet traffic used in MB
* `is_ultimate` — plan for the current month (Ultimate - 1, Surf - 0)