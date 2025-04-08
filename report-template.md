# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### NAME HERE

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
When I first submitted my predictions, I encountered issues with the submission format. Specifically, I realized that the predictions contained negative values, which are not valid for bike counts. To address this, I had to apply a transformation to set all negative predictions to zero before submitting them. 
### What was the top ranked model that performed?
WeightedEnsemble_L3 model outperformed other models, it had the lowest RMSE value of -33.558823 which means it generalizes to the validation data the best compared to other models.## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
exploratory analysis revealed patterns in bike-sharing demand, such as higher demand during certain months, hours of the day, and weather conditions. I added features such as hour of the day, day of the week, and temperature categories. 
### How much better did your model preform after adding additional features and why do you think that is?
TODO: it got better probably because the added features allowed the model to understand the patterns better

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: The performance dropped

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: I would do it with the second model as it was the best performing one. 

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|

model	time	preset	extra	score
0	initial	600	best_quality	no	1.80597
1	add_features	200	best_quality	no	1.95793
2	hpo	720	best_quality	yes	0.43825

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.
(unable to copy and paste the line plot but it is in the notebook)
![model_train_score.png](img/model_train_score.png)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

(unable to copy and paste the line plot but it is in the notebook)
![model_test_score.png](img/model_test_score.png)

## Summary
TODO: Add your explanation
Three models were made, given different amount of time for training, and features were added as new models were made
