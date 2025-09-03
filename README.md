# Flight Booking Price Prediction

## Overview

This project predicts **flight ticket prices** based on multiple factors such as airline, source city, destination city, number of stops, travel class, and days left before departure.
The dataset used is `Flight_Booking.csv`, and various machine learning models were applied to compare performance.

## Dataset

* **File:** `Flight_Booking.csv`
* **Features:**

  * `airline` – Name of the airline
  * `source_city` – Departure city
  * `destination_city` – Arrival city
  * `departure_time` – Time of departure (Morning/Afternoon/Night)
  * `arrival_time` – Time of arrival
  * `stops` – Number of stops
  * `class` – Travel class (Economy/Business)
  * `days_left` – Days left for departure
  * `price` – Target variable (Ticket price)

## Steps Performed

1. **Data Preprocessing**

   * Removed unwanted columns (`Unnamed: 0`)
   * Checked for missing values and summary statistics
   * Encoded categorical features using `LabelEncoder`
   * Standardized numerical features with `StandardScaler`

2. **Exploratory Data Analysis (EDA)**

   * Visualized **Airline vs Price**, **Days Left vs Price**
   * Count plots for airline, source/destination cities, departure/arrival times, class, and stops
   * Correlation heatmap to check multicollinearity
   * Variance Inflation Factor (VIF) to verify feature redundancy

3. **Model Training**

   * **Linear Regression**
   * **Decision Tree Regressor**
   * **Random Forest Regressor**

4. **Evaluation Metrics**

   * R² Score
   * Mean Absolute Error (MAE)
   * Mean Absolute Percentage Error (MAPE)
   * Mean Squared Error (MSE)
   * Root Mean Squared Error (RMSE)

## Results

* **Linear Regression**: Good for baseline, but struggled with complex patterns
* **Decision Tree**: Improved results but prone to overfitting
* **Random Forest**: Best model with the highest accuracy and lower errors

## Tech Stack

* **Python**
* **Pandas, NumPy** – Data handling
* **Matplotlib, Seaborn** – Visualization
* **Scikit-learn** – ML Models & Preprocessing
* **Statsmodels** – VIF Analysis
