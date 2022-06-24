# Binary_Classifier_Model_DeepLearning

This is an exercise which uses a example VC firm's data of startups that received funding and the goal is to help them determine what information is useful to classify the startup as successful or not. This code will allow you to use machine learning and neural networks to create a binary classifier model that will help predict whether or not an applicant will be successful. 
<br />

## Technologies

This project leverages python 3.7 in a jupyter notebook ipynb file
<br />

## Installation Guide

Before running the application first install the following dependencies.<br />

 pip install pandas<br />
 pip install --upgrade tensorflow<br />
 python -c 'import tensorflow as tf;print(tf.keras.__version__)'<br />
 from tensorflow.keras.layers import Dense<br />
 from tensorflow.keras.models import Sequential<br />
 from sklearn.model_selection import train_test_split<br />
 from sklearn.preprocessing import StandardScaler,OneHotEncoder<br />


## Findings/Analysis
First, we determine which columns of the data are int64 and which are objects. The object columns are then created into a list of categorical variables. A new dataframe is then created with the encoded data and concatenated back with the int64 column data. This data is then split into training and testing datasets and scaled using StandardScaler. All of this is then compiled. <br />

-All 3 tests used 1 nueron as the output.<br />
-The original test contained 2 hidden layers and 50 epochs. This resulted in a loss of 0.5539 and an accuracy of 0.7294<br />
-The Alternative Model 1 contained only 1 hidden layer and 30 epochs. This resulted in a loss of 0.5560 and an accuracy of 0.7296<br />
-The Alternative Model 2 contained 3 hidden layers and 70 epochs. This resulted in a loss of 0.5553 and an accuracy of 0.7311
-In conclusion, Alternative Model 2 resulted in the highest accuracy of 0.7311 and a median loss of 0.5553 in comparison to the other models.

<br />

## Contributors

Jeffrey Liu : Dev
UCB Fintech - Provided initial resources

<br />
## License
Trilogy Technology 
UCB Fintech Extension Program



