# Monthly-Flight-Passengers-Prediction-Using-LSTM-Model-on-Inbuilt-Seaborn-Dataset
Pytorch based Long Short-Term Memory(LSTM) model on total passengers forecasting using time-series Seaborn Flight Passengers data. 

## Pre-Requests:
### Download:
**.** Repository:
                
                **1.** If you want to download directly there is a download button on the right corner of this repository or else use Command Prompt. 
                
                **2.** In Windows first install Git software Open Command Prompt--> git clone https://github.com/Nutakki2259/Monthly-Flight-Passengers-Prediction-Using-LSTM-Model-on-Inbuilt-Seaborn-Dataset.git
                
                **3.** In Anaconda Open Command Prompt--> conda activate <conda environment name> --> git clone https://github.com/Nutakki2259/Monthly-Flight-Passengers-Prediction-Using-LSTM-Model-on-Inbuilt-Seaborn-Dataset.git

Note: The folder will be saved at the place where the command prompt shows activate for example: '(Python3.7) C:\Users\pradeep>git clone https://github.com/Nutakki2259/Monthly-Flight-Passengers-Prediction-Using-LSTM-Model-on-Inbuilt-Seaborn-Dataset.git'

**.** Dataset: The dataset is directly an inbulit of Seaborn as 'flights'. So, directly downloaded in the hupyter notebook.

## 1. Data Description
The dataset is an inbuilt data from Seaborn as 'flights' dataset. This dataset provides data from 1949 January. The dataset has three columns: year, month, and passengers. The passengers column contains the total number of traveling passengers in a specified month.

## 2. Loading and Splitting Dataset
The dataset is directly loaded from Seaborn as there is no requirement of saving the data. The columns are well structured and no need of cleaning data. The dataset is a single set of consisting (144x3) dimension. This dataset is converted into train: 132 and test: 12 elements.

## 3. Convert the Data into X,y
The dataset of train for the model is divided into input (X) and target (y) values. This divided into sequences of 12 of the train dataset for the model.

## 4. Designing LSTM Network for the Predition of Future Passengers Data 
Initialise the data layers for the LSTM, sequence length, hidden and feature size. As it is require to reset the state after every epoch of turn to analyse again the data as clear. Get the test data time step that is required and sent to linear layer to forecast the future.

## 5. Tuning Hyperparameters of the Model and Loss Calculation
The performance of the model depends on fine-tuning of the hyperparameters during training. The loss is calculated as mean square error that is decreasing with the epochs. The model shows a good performance in prediction of the data.

## 6. Validating Test Data Points for the Prediction by the LSTM Model
The **Pre-Trained Model** defines the test data on the understanding parameteres. The data points are chosen as 12 because the train has 132 elements resulting total dataset elements as 144.

## 7. Plot for the Predicted Flight Passengers 
The plot is between the original dataset values and predicted data by the network. The model predicts better on continuous tuning of hyperparameters for time-series dataset.
![Predictions](https://github.com/Nutakki2259/Monthly-Flight-Passengers-Prediction-LSTM/blob/main/predictions.PNG)

### References
https://www.curiousily.com/posts/time-series-forecasting-with-lstm-for-daily-coronavirus-cases/


