# Time-series-Prediction-LSTM-
## DATA :- Federal Reserve Economic Data(FRED) 'Alocoholic beverages sales data'
## It contains the alcoholic sales in millions(USD) every month from 1992-January
![](https://github.com/Yashwanthkumar11/Time-series-Prediction-LSTM-/blob/master/.ipynb_checkpoints/dataset.png)

## Plot of the data
![](https://github.com/Yashwanthkumar11/Time-series-Prediction-LSTM-/blob/master/.ipynb_checkpoints/plot.png)

## Data preparation for training
We can see that there is yearly trend in the data which suggests us to use a sequence of 12months as one input sequence to LSTM and the label for that input sequence is the value following that input sequence.

Such a tuple of (inputs,labels) are used where these inputs are the sequences of 12months each, which go into LSTM model as inputs and compared against the labels using Mean-squared error.

## Analysis of the predictions of the trained model

Inorder to check the performance of the model, the data was intially split into training set and test set where the model training was performed on training set and predicted for test set range of values.

The picture below indicates how well the model has learnt the trend where the orange curve is the model predictions and blue curve is the actual data.

![](https://github.com/Yashwanthkumar11/Time-series-Prediction-LSTM-/blob/master/.ipynb_checkpoints/plot1.png)

## Forecasting 

Forecasting or predicting the future values is also done in the similar way as above but here the model was trained on the entire dataset i.e without train-test split.

![](https://github.com/Yashwanthkumar11/Time-series-Prediction-LSTM-/blob/master/.ipynb_checkpoints/plot2.png)

For clear understanding, please refer to the python notebook file in this repo.
