# Daily-Minimum-Temperatures-Forecasting-using-LSTM
This project demonstrates how to use a Long Short-Term Memory (LSTM) neural network for time series forecasting of daily minimum temperatures in Melbourne, Australia. The model is built using TensorFlow/Keras and trained on a historical temperature dataset.

The goal is to predict future temperature values based on previous time steps using an LSTM deep learning model.

---

📂 Dataset
Name: Daily Minimum Temperatures in Melbourne

Source: UCI Machine Learning Repository

File: Daily_minimum_temperatures.csv

The dataset contains two columns:

Date

Minimum Temperature (°C)

---

echnologies Used
Python 3.x

TensorFlow / Keras

NumPy

Pandas

Matplotlib

Scikit-learn

---

🚀 Project Workflow
1. Data Preprocessing
Load the dataset using Pandas.

Handle missing values and convert data to numeric form.

Apply Min-Max normalization using MinMaxScaler.

2. Sequence Reconstruction
Transform the time series into supervised learning data using sliding windows of the last N days to predict the next day.

3. Train-Test Split
Split the data into 70% training and 30% testing sets.

4. Build the LSTM Model
Stack three LSTM layers with Dropout to prevent overfitting.

Output layer is a Dense layer with one unit for regression.

5. Train the Model
Use the Adam optimizer and Mean Squared Error loss.

Train for 20 epochs.

6. Evaluate & Visualize
Make predictions on the test set.

Compute Root Mean Squared Error (RMSE).

Plot original vs. predicted values.

---

📈 Results Example
After training, the model generates predictions that follow the general trend of the actual temperature values.

---
📄 How to Run
1. Clone the Repository
git clone https://github.com/MParsaMo/temperature-forecast-lstm.git
cd temperature-forecast-lstm

2. Install Dependencies
pip install -r requirements.txt

3. Place Dataset
Download the CSV file and place it in the project directory.
File name: Daily_minimum_temperatures.csv

4. Run the Code
python temperature_forecast.py

---

🔑 Key Parameters
| Parameter           | Value                        |
| ------------------- | ---------------------------- |
| Previous Time Steps | 5                            |
| LSTM Layers         | 3 layers (100, 50, 50 units) |
| Dropout Rates       | 0.4, 0.3, 0.3                |
| Batch Size          | 32                           |
| Epochs              | 20                           |

---

📊 Performance Metric
Root Mean Squared Error (RMSE) is used to evaluate model performance.

---

📌 Notes & Next Steps
✅ You can try:

Tuning the number of previous time steps.

Adding more LSTM layers or increasing units.

Applying early stopping or validation splits.

Using more advanced sequence models (GRU, Transformer).

---

🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request.

---








