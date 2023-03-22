# Project description

Beta Bank's customers are leaving, each month, little by little. The bankers discovered that it is cheaper to save existing customers than to attract new ones. We need to predict if a customer will leave the bank soon. You have the data about the past customer behavior and termination of contracts with the bank. Creates a model with the maximum F1 value possible. To pass the review, you need a **F1 value of at least 0.59**. Check F1 for the test set. Also, you should measure the AUC-ROC metric and compare it to the F1 value

## Project instructions.

1. Download and prepare the data. Explain the procedure. 
2. Examine the balance of classes. Trains the model without taking imbalance into account. Briefly describe your findings. 
3. Improves the quality of the model. Make sure you use at least two approaches to correct the class imbalance. Use training and validation sets to find the best model and the best set of parameters. Train different models in the training and validation sets. Find the best. Describes briefly your findings. 
4. Compute a final test.

## Data description

**Features**
* `RowNumber` — data string index
* `CustomerId` — unique customer identifier
* `Surname` —surname
* `CreditScore` — credit value
* `Geography` — country of residence
* `Gender` — sex
* `Age` — age
* `Tenure` — maturity period for a client's fixed deposit (years)
* `Balance` — account balance
* `NumOfProducts` — number of banking products used by the client
* `HasCrCard` — the customer has a credit card
* `IsActiveMember` — client activity
* `EstimatedSalary` — estimated salary

**Target**
* `Exited`: The client has left