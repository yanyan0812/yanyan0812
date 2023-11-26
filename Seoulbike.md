# Seoul Bike Sharing Demand Prediction

This project aims to predict the demand for bike sharing in Seoul using LSTM (Long Short-Term Memory) networks. LSTM is a type of recurrent neural network suitable for time series prediction. The dataset contains various features like temperature, humidity, wind speed, visibility, dew point temperature, solar radiation, rainfall, snowfall, seasons, holiday, and functioning day.

## Project Structure

The code includes the following steps:

1. Loading the Seoul bike sharing dataset and performing necessary data preprocessing.
2. Conducting exploratory data analysis (EDA) to understand the data better and prepare it for modeling.
3. Splitting the data into training and testing sets.
4. Normalizing the features using `MinMaxScaler`.
5. Creating time-series sequences to be used as inputs for the LSTM model.
6. Building and training the LSTM model on the preprocessed data.
7. Evaluating the model using RMSE (Root Mean Square Error) and R² score.
8. Visualizing actual vs. predicted demand to assess the model's performance.

## Requirements

- Python 3.6 or above
- TensorFlow 2.4
- Keras
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

## Dataset

The dataset is the Seoul Bike Sharing Demand dataset, which includes the following columns:

- Date
- Rented Bike Count
- Hour
- Temperature
- Humidity(%)
- Wind speed (m/s)
- Visibility (10m)
- Dew point temperature(°C)
- Solar Radiation (MJ/m2)
- Rainfall(mm)
- Snowfall (cm)
- Seasons
- Holiday
- Functioning Day

## Usage

To replicate the findings and the LSTM model, follow these steps:

1. Install the required libraries as mentioned in the `Requirements` section.
2. Load the dataset using pandas and preprocess the data as described in the code.
3. Run the EDA code to visualize and understand the data distributions and correlations.
4. Execute the model training code to build the LSTM model.
5. Evaluate the model using the provided metrics.
6. Visualize the predictions against the actual data.

## Model Training

The LSTM model is trained with the following architecture:

- Bidirectional LSTM layer with 128 units.
- Dropout layer with a rate of 0.2 to prevent overfitting.
- Dense output layer with a sigmoid activation function.

The model is compiled with the Adam optimizer and Mean Squared Error loss function.

## Results

The trained model's performance is evaluated using RMSE and R² score. The visualization of the actual vs. predicted demands is provided to assess the model's predictive capabilities visually.

## Contributing

Contributions to this project are welcome. You can suggest improvements to the code, propose new visualizations, or enhance the model's performance.

## Contact

For any queries or discussions related to this project, please reach out via Email yanyan08@ewahin.net
