# Machine_Learning_2023_OVGU

##  Machine Learning for Chemical Engineering
Welcome to the course on Machine Learning for Chemical Engineering! In this course, we will explore the fascinating intersection of machine learning and chemical engineering and understand how these two fields can synergistically work together to solve complex problems and optimize processes in the chemical industry.

##  Class Tasks

### Task 1/2
Develop a kNN model for regression to predict the bioconcentration factor (BCF) for the given data

perform data cleaning if required and define corresponding variables for [inputs /features] and [corresponding output (Experimental values)]

do cross validation with different k values and visualize (R2_square vs k and MSE vs k) to know what k value performs best on your testing data.

final trained model using all the data points with your k value

### Task 3
Develop a Generalized Linear regression model to predict the Internal energy (U) of saturated vapor for the given pressure data (P)

perform data cleaning if required and define corresponding variables for [inputs /features] and [corresponding output (Experimental values)] 

Input/Feature is Pressure and Output is Internal Energy for saturated vapor

do cross validation with different values of degree of polynomial and visualize (R2_square vs degree of polynomial and MSE vs degree of polynomial) to know what 'degree of polynomial' value performs best on your testing data.

train your final model using all the data points with your 'degree of polynomial value

### Task 4
Develop a Deep Neural Network model to predict the PE for the given input data in a Combine Cycle Power Plant (CCPP)
input data ; Ambient Temperature (AT), V(V), Atmospheric Pressure (AP), Relative Humidity (RH), Exhaust Vacuum (V)
output data ; Electric Power (PE).

perform data cleaning if required and define corresponding variables for [inputs /features]  and [corresponding output (Experimental values)]

Input/Features are AT,V,AP,RH and Output is PE 

Use Pytorch to perform a Feed Forward Neural Network.

Do cross validation using GridsearchCv.

Train your final model using all the available data points with optimized hyperparamters (found in best model of GridsearchCv.

Write code to save your final trained model and download the saved file with name 'your_name_final_model.h5' to submit along with this python file.

At last write the final function in exactly the same format as taught in class.

