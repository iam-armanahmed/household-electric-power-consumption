
# Predict weekely household power comsumption

### Problem Statement
Problem : Given input data for a week (7 Days ~ & timesteps), predict the mean global_active_power for the next week.  

Data Source : [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

### Expploratoy Data Analysis  (Please see the jupyter notebook for an in-depth analysis) :
- The data consists of missing values which were replaces with mean grouped over yearly values.
- The data was resampled on daily level. 
- - **Note** : **Had just 1443 observations and 7 features**, the data is very less for training deep learning models.

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


