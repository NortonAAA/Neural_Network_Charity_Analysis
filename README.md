# Neural Network Charity Analysis
Module 19 Bootcamp Challenge

## Purpose
The purpose of this analysis was to develop a neural network using historical data to develop a learning model that could predict up to 75% accuracy the success of an organization's use of charity funds.
## Results
Historical data from the organization was broken down into 2 steps. Data preprocessing and the Model development
### Data Preprocessing
- Target of the model was whether a organization was successful or not (Y/N?)
- Features of the model was determined to be:

![](https://github.com/NortonAAA/Neural_Network_Charity_Analysis/blob/main/images/features.png)

- Other variables that were drop and of no value were the EIN and the Name shown below
![](https://github.com/NortonAAA/Neural_Network_Charity_Analysis/blob/main/images/drop_variables.png)

Due to the spread of the Classifcation and Application Type features, the unique values were combined to allow for more even processing.
### Compiling, Training, and Evaluating the Model
The initial model was developed with an input layer, 2 hidden layers, with 80 nodes on hidden layer 1 and 30 nodes on hidden layer 2 summary is shown below:
![](https://github.com/NortonAAA/Neural_Network_Charity_Analysis/blob/main/images/model_original_summary.png)

The Rectified Linear Activiation Functions were used as to perserve the positive values and prevent impact of negative values.

The accuracy of this original model was below:
![](https://github.com/NortonAAA/Neural_Network_Charity_Analysis/blob/main/images/model_original_accuracy.png)

In the Optimization of the model, we attempted several aspects of:
- Changing number of layers and number of nodes to tune the model
- Increased and reduced the number of Classificationa and Application Types to give the model more or less features.

At best this highest accuracy achevied was on model 4 run with 2 hiddent layers with 300 and 100 nodes respectively. Yielding only a slight increase:
![](https://github.com/NortonAAA/Neural_Network_Charity_Analysis/blob/main/images/Optimization_run4.png)

## Summary
Overall, we were not able to get to the desired 75% accuracy level desired above. There is an opportunity to simpliy the number of classifcation features. Instead of putting lower counts into arbitrary "Other" bucket, it would be better to review the actual classifications an put all 1-2 values spread into a better classification. Determining how the classification is determined could provide a better understanding of features to breakout.