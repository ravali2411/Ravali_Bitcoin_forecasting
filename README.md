# Ravali_Bitcoin_forecasting
Bitcoin Time Series Forecasting

This project focuses on forecasting Bitcoin prices using deep learning models like Recurrent Neural Networks (RNNs), Long Short-Term Memory (LSTM), and Gated Recurrent Units (GRUs). The key objectives were:

1. Evaluate the performance of RNN, LSTM, and GRU models for Bitcoin price prediction.

2. Preprocess and prepare the Bitcoin price data for time series forecasting.
   
3. Train and optimize the models using appropriate hyperparameters.

4. Analyze and visualize the forecasting results to identify the best-performing model.
   
Data:

The project utilized Bitcoin price data obtained from the yfinance library, which provides accurate historical and real-time financial data.
1
 The raw data was preprocessed using MinMaxScaler for normalization to enhance model performance and predictability.
1

Data Preprocessing

The following data preprocessing steps were performed:

Joined the Bitcoin price data with additional relevant datasets (if any).

Extracted relevant features like open, close, high, and low prices.

Normalized the data using MinMaxScaler to scale values between 0 and 1.


Split the data into training and testing sets (67% for training, 33% for testing).


Model Selection and Training:

Three deep learning models were selected for Bitcoin price forecasting:

1. RNN (Recurrent Neural Network): A basic recurrent network suitable for capturing short-term dependencies.
   
2. LSTM (Long Short-Term Memory): Excels at capturing long-term dependencies and mitigating the vanishing gradient problem.

3.GRU (Gated Recurrent Unit): Computationally efficient and adept at capturing short- to medium-term trends.

The models were trained using the preprocessed training data, with hyperparameters like hidden size, number of epochs, and lookback window optimized for each model.

The lookback window sizes of 3 and 7 were explored to capture short-term and medium-term patterns, respectively.

Evaluation and Visualization

The trained models were evaluated on the test data using the Root Mean Squared Error (RMSE) metric, which quantifies the difference between predicted and actual values.

The predictions were visualized against the actual values to assess the model's performance visually.

Results

The best-performing models achieved the following RMSE scores on the test data:

RNN: 0.0708

LSTM: 0.0282

GRU: 0.0296

The LSTM model outperformed the others, achieving the lowest RMSE score of 0.0282, indicating its superior forecasting ability for Bitcoin prices.

Teamwork

This project was a collaborative effort involving:

1.Jaswanth Buggana - Data preprocessing, LSTM model implementation

2.Nihar Lonka- RNN model implementation, visualization

3.Ravali Venkatayogi - GRU model implementation, hyperparameter tuning

The team effectively divided responsibilities, combined individual contributions, and worked cohesively to deliver the project.

Future Work

Potential areas for future research include incorporating additional features like trading volume, sentiment analysis, and exploring advanced deep learning architectures like attention mechanisms and transformer models for improved Bitcoin price forecasting.
