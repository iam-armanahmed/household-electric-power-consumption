
# Predict weekly household global active power consumption 

### Problem Statement
Problem : Given input data from previous week (7 Days ~ 7 timesteps), predict the mean global_active_power for the next week.  

Data Source : [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

### Exploratoy Data Analysis  (Please see the jupyter notebook for an in-depth analysis)

### Model Results

#### CNN Model

![CNN Model training history](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/CNN-Modelloss_and_metric.png)

![CNN Model prediction vs true values plot](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/CNN-Modelpred_vs_true.png)

#### LSTM Model

![LSTM Model training history](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/LSTM-Modelloss_and_metric.png)

![LSTM Model prediction vs true values plot](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/LSTM-Modelpred_vs_true.png)

#### CNN-LSTM Model

![CNN-LSTM Model training history](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/CNN-LSTM%20Modelloss_and_metric.png)

![CNN-LSTM Model prediction vs true values plot](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/CNN-LSTM%20Modelpred_vs_true.png)

#### ConvLSTM Model

![ConvLSTM Model training history](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/ConvLstm2D%20Modelloss_and_metric.png)

![ConvLSTM Model prediction vs true values plot](https://github.com/iam-armanahmed/household-electric-power-consumption/blob/master/Images/ConvLstm2D%20Modelpred_vs_true.png)


Analysis of CNN, LSTM, CNN-LSTM and ConvLSTM Models:

> Model Performance Evaluation Plots :

> 1 - Plotting the models loss (MSE) and metric (RMSE) indicates a good fit rather than over-fit or an undner-fit. <br>
> > 2 - It is interesting to observe that the training loss (MSE) and metric (RMSE) is more than testing. It can be stated that training data consists of data with more complex underlying latent structure as compared to testing data. <br>

True values VS Preicted Values

> > 1- Time dealy in learning.  <br>
> > 2- It is observed that ConvLSTM2D model performs much better (RMSE) than other models (CNN, LSTM and CNN-LSTM). But the data available for training was very less considering deep learning models, hence given more data, model performance can be improved to make more accurate predictions (weekly prediction).


