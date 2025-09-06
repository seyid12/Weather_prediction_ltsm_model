# weather_prediction_ltsm_model

Great idea! A README.md file makes your project understandable and accessible for both you and others.

Here's a comprehensive README.md file ready for your project. You can copy and paste it directly into your GitHub repository.

Markdown

# ☀️ LSTM-Based Weather Forecast for Spanish Cities

This project uses **LSTM (Long-Short-Term Memory)** neural networks to predict temperatures for five major cities in Spain (Valencia, Madrid, Bilbao, Barcelona, ​​Seville). The model is trained to predict the temperature for the next hour by analyzing the past 24 hours of data.

## Project Purpose and Features

* **Time Series Analysis:** Predicting future temperatures using historical weather data.

* **Deep Learning Model:** Training a separate LSTM model for each city and evaluating the performance of these models.
* **Multiple Important Features:** Using features other than temperature in the prediction model, such as pressure, humidity, wind speed, and cloud cover.
* **Model Performance Evaluation:** Measuring model accuracy with the **RMSE (Root Mean Square Error)** metric.

## Model Performance

The trained models achieved high performance with low RMSE values ​​on the test data. These values ​​represent the average deviation of the predictions from the actual temperature.

| City | Test RMSE (°C) |
| :--- | :--- |
| **Bilbao** | **0.88** |
| Madrid | 0.95 |
| Valencia | 0.98 |
| Barcelona | 0.99 |
| Seville | 1.07 |

The best-performing Bilbao model predicted with an average error of just 0.88 °C.

## Technologies Used

* Python: The project's primary programming language.
* Pandas: Used for data processing and analysis.
* NumPy: Used for numerical operations and array manipulations.
* TensorFlow / Keras: Used to build and train deep learning models.
* Scikit-learn: Used for data normalization (MinMaxScaler).

## File Structure

The basic file structure of the project is as follows:

/
├── weather_features.csv # Original dataset

├── weather_prediction_project.ipynb # Kaggle notebook (main code)

├── trained_models/ # Folder where trained models are stored

│ ├── lstm_model_valencia.h5

│ └── ... (models of other cities)

├── README.md # This file


## Running the Project

1. Clone this repository to your local machine: `git clone <your_repository_address>`
2. Install the necessary libraries: `pip install pandas numpy tensorflow scikit-learn`
3. Open the `weatherpredictionproject.ipynb` file in Jupyter or a similar environment and run the steps in order.

---
