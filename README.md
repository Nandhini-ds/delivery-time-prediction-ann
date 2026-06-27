# delivery-time-prediction-ann
# Deep Neural Network (ANN) model for predicting food (Porter) delivery time.
## Project Overview

This project develops a Deep Neural Network (ANN) regression model to predict food delivery time using delivery-related data. The objective is to improve the accuracy of estimated delivery times (ETA), helping logistics platforms provide reliable delivery estimates, enhance customer satisfaction, and support efficient delivery operations.

The project covers the complete machine learning workflow, including data preprocessing, feature engineering, model development, training, evaluation, and performance optimization using techniques such as feature scaling, Batch Normalization and Early Stopping.
## About Porter

Porter is one of India's leading intra-city logistics platforms, connecting restaurants, customers, and delivery partners to provide fast and reliable on-demand delivery services. With operations across multiple cities, Porter aims to deliver orders efficiently while ensuring a seamless customer experience.

## Business Problem

Accurately estimating food delivery time is a critical challenge for logistics platforms. Delivery time is influenced by several factors, including order characteristics, restaurant location, customer location, delivery partner availability, traffic conditions, and operational constraints.
The objective of this project is to build a Deep Neural Network (ANN) regression model that predicts the Estimated Time of Arrival (ETA) for food deliveries using delivery-related features. Improving ETA predictions helps logistics companies provide reliable delivery estimates, enhance customer satisfaction, optimize delivery operations, and support better decision-making.

## Dataset Description
The dataset contains historical food delivery order information collected from Porter. Each record represents a single delivery order and includes details about the restaurant, order characteristics, delivery partner availability, and estimated travel time.
| **Feature**                                    | **Description**                                                                                                       |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `market_id`                                    | Integer identifier for the market where the restaurant is located.                                                    |
| `created_at`                                   | Timestamp when the order was placed.                                                                                  |
| `actual_delivery_time`                         | Timestamp when the order was delivered. Used to calculate the target variable (delivery time).                        |
| `store_primary_category`                       | Primary category of the restaurant.                                                                                   |
| `order_protocol`                               | Integer code indicating how the order was placed (e.g., Porter app, phone call, pre-booked, or third-party platform). |
| `total_items`                                  | Total number of items in the order.                                                                                   |
| `subtotal`                                     | Total order value before taxes and fees.                                                                              |
| `num_distinct_items`                           | Number of unique items in the order.                                                                                  |
| `min_item_price`                               | Price of the least expensive item in the order.                                                                       |
| `max_item_price`                               | Price of the most expensive item in the order.                                                                        |
| `total_onshift_partners`                       | Number of delivery partners on duty when the order was placed.                                                        |
| `total_busy_partners`                          | Number of delivery partners currently occupied with other deliveries.                                                 |
| `total_outstanding_orders`                     | Total number of pending orders at the time the order was placed.                                                      |
| `estimated_store_to_consumer_driving_duration` | Estimated driving time from the restaurant to the customer's location.                                               
## Project Workflow

1. Data Exploration
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
   * Created date and time-based features from the `created_at` timestamp.
   * Calculated the target variable (delivery time) using the difference between `created_at` and `actual_delivery_time`.
4. Data Preprocessing
   * One-Hot Encoded categorical features.
   * Standardized numerical features using `StandardScaler`.
5. Train-Validation-Test Split
6. Baseline ANN Model Development
7. Improved ANN Model with Batch Normalization, L2 Regularization, Adam Optimizer, and Early Stopping
8. Random Forest Regression Model for Performance Comparison
9. Model Evaluation and Performance Comparison
10. Final Model Selection
    
## Technologies Used
* **Programming Language:** Python
* **Development Environment:** Google Colab
* **Libraries:**

  * NumPy
  * Pandas
  * Matplotlib
  * Scikit-learn
  * TensorFlow / Keras

