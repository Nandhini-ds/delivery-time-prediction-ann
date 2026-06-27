# delivery-time-prediction-ann
# Deep Neural Network (ANN) model for predicting food delivery time.
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
| Feature | Description |
|---------|-------------|
| `market_id` | Identifier for the market where the restaurant is located. |
| `created_at` | Timestamp when the order was placed. |
| `actual_delivery_time` | Timestamp when the order was delivered. |
| `store_primary_category` | Primary category of the restaurant. |
| `order_protocol` | Order placement method. |
| `total_items` | Total number of items in the order. |
| `subtotal` | Total order value before taxes and fees. |
