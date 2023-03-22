# Project description

You work for the OilyGiant mining company. Your task is to find the best place for a new well.
Steps to choose the location:
* Collects the parameters of the oil well in the selected region: quality oil and volume of reserves;
* Build a model to predict the volume of reserves in new wells;
* Selects the oil wells with the highest estimated values;
* Choose the region with the highest total benefit for oil wells selected.

You have data on crude oil samples from three regions. The parameters are already known for each oil well in the region. Create a model that helps choose the region with the highest profit margin. Analyze potential benefits and risks using the bootstrap technique.

## Project Instructions
1. Download and prepare the data. Explain the procedure.
2. Train and test the model for each region:
     * 2.1. Split the data into a training set and a validation set in a 75:25 ratio.
     * 2.2. Train the model and make predictions for the validation set.
     * 2.3. Saves the predictions and correct answers for the validation set.
     * 2.4. Displays on the screen the average volume of forecasted reserves and the RECM of the model.
     * 2.5. Analyze the results.

3. Prepare for profit calculation:
    * 3.1. Stores all key values for calculations in separate variables.
    * 3.2. Calculate the volume of reserves sufficient to develop a new well without losses. Compare the value obtained with the average volume of reserves for each region.
    * 3.3. Provides the findings on readiness for the profit calculation step.

4. Write a function to calculate the profit for a set of selected oil wells and model the predictions:
    * 4.1. Choose the wells with the highest values of predictions.
    * 4.2. Summarizes the target volume of reserves according to these predictions
    * 4.3. It provides the findings: suggests a region for the development of oil wells and justifies the choice. Calculate the profit for the volume of reservations obtained.

5. Calculate risks and rewards for each region:
    * 5.1. Use the bootstrapping technique with 1000 samples to find the profit distribution.
    * 5.2. Find the average profit, the 95% confidence interval, and the risk of loss. The loss is a negative gain, calculate it as a probability and then express it as a percentage.
    * 5.3. It provides the findings: suggests a region for the development of oil wells and justifies the choice.

## Data description

Geological exploration data for the three regions is stored in files:

* `geo_data_0.csv`
* `geo_data_1.csv`
* `geo_data_2.csv`
* `id` — unique oil well identifier.
* `f0`, `f1`, `f2` — three features of the points (their specific meaning is not important, but the features themselves are significant).
* `product` - volume of reserves in the oil well (thousands of barrels).

## Conditions:
* Only linear regression is suitable for model training (the rest are not predictable enough).
* When exploring the region, a survey of 500 points is carried out with the selection of the best 200 points for profit calculation.
* The budget for the development of 200 oil wells is 100 million dollars.
* A barrel of raw materials generates 4.5 USD of income. The income from a unit of product is 4,500 dollars (the volume of reserves is expressed in thousands of barrels).
* After the risk assessment, keep only the regions with loss risk below 2.5%. Of those that fit the criteria, the region with the highest average profit should be selected.
* The data is synthetic: the details of the contract and the characteristics of the well are not published.