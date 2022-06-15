# Deep-Learning

### Deep Learning Homework Assignment
  In this asignment we created and trained a custom LSTM RNN that uses a 10 day window of Bitcoin fear and greed index values to predict the 11th day closing price.
We also built and trained a custom LSTM RNN that uses a 10 day window of Bitcoin closing prices to predict the 11th day closing price.
In doing so, we imported data from our csv files, prepared this data for training and testing, built and trained custom LSTM RNN's, and evaluated the performance of these models.

### Data Preperation, Building and Training our Models
  For our data preperation we used the window_data function to generate the specific X and y values for our models. We also split the data into 70% for training and 30% for testing and applied the MinMaxScaler to the X and y values. We also reshaped the X_train and X_test data for the models. After these steps, we defined our model architectures, compiled our models, and fit our models to the training data.
  
### Evaluating our Models performances
  We evaluated each model using the X_test and y_test data and we used the X_test data to make predictions. We create a DataFrame of Real (y_test) vs predicted values and we plotted the real vs predicted values as a line chart. It seems as though the model using the Bitcoin closing prices had less loss at .0130 compared to .0546 for the model using the fear and greed index. Our closing price model also tracks the actual values better, and a window of 10 days worked better for both models in our case.
  
