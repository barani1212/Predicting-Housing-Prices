# Predicting-Housing-Prices

# Housing Price Prediction

This project focuses on predicting the median house value in various regions based on multiple features like housing median age, total rooms, total bedrooms, population, households, and median income. The prediction is carried out using various regression models, and the best model is selected based on performance metrics.


## Installation

To set up this project on your local machine, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/barani1212/housing-prediction.git
   cd housing-prediction

2. **Create a virtual environment (optional but recommended)**:
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. **Install dependencies:**
   pip install -r requirements.txt

Usage
1. Train the Models
The model_training.py script trains several regression models on the housing dataset and selects the best one based on Root Mean Squared Error (RMSE).

Run the script:
python models/model_training.py
2. Predict House Values
Use the prediction_function.py script to predict the median house value based on custom inputs. The script uses the best model identified during training.

Example usage:
from models.prediction_function import pred

predicted_value = pred(52.0, 1627.0, 280.0, 565.0, 259.0, 3.8462)
print(f"Predicted Median House Value: ${predicted_value:.2f}")
3. Explore the Data
The data_exploration.ipynb notebook contains code for exploring the dataset, visualizing the relationships between variables, and understanding the data better.
