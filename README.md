# Porter-NN
### Problem
Porter, India's largest marketplace for intra-city logistics, is revolutionizing the
delivery sector with technology-driven solutions.

● This case focuses on leveraging neural networks to accurately predict delivery
times, a critical aspect of customer satisfaction in logistics.

● With a dataset encompassing various aspects of orders and deliveries, Porter
aims to refine its delivery time estimations.

### Objective

● Analyzing this dataset to provide significant insights into delivery dynamics,
efficiency bottlenecks, and optimization opportunities.

●Build a regression model and evaluate its performance, and provide insights for optimizing delivery
operations.

### Techniques Used
#### Data Wrangling
Data Cleaning, Duplicate Value Check, Missing Values Treatment, Feature Engineering, Data Encoding, Detecting and Removing Outliers 

#### Data Visualisation
Univariate Analysis using countplot, kdeplot, histplot

Bivariate Analysis using barplot. 

#### Regression Model
Neural Networks with adam optimiser, L2 Regulariser, Learning Rate Decay and Dropout.


### Results
The model performs best on first 3 to 4 epochs in model1 and  model2 after that it doesnot make any significant improvement.

This could be because for the same dish prepared by same restraunt delivery to same location may differ every time thus the variation in input.

model1 with adam optimiser and L2 reguraliser gives train loss: 148.9552 and  validation loss: 154.4703 

model2 with additional hyperparameter tuning of adam optimiser and using Learning Rate Decay gives training loss: 151.7911  and  validation loss: 156.8335  

model3 uses dropout rate 0f 0.3 and Leaky Relu as activation function gives training loss: 178.5572 and  validation loss: 161.0964  

model4 uses same parameters as model 3 but is used on different train validation and test size gives training loss: 179.9830  and  validation loss: 161.9616 

The model with least Mean absolute error is model1 with MAE of 9.90346579070213

