# ✈️ Propensity Modeling for Travel Ticket Purchase Prediction

## Overview

This project involves building a machine learning-based propensity model for an aviation company to predict the likelihood of customers purchasing travel tickets. The objective is to optimize digital advertising by targeting users with a high probability of purchase based on their behavioral data collected through a social networking platform.

## Problem Statement

The aviation company seeks to improve customer acquisition efficiency by shifting from broad outreach to personalized digital marketing. Since advertising costs are significant, it's crucial to identify potential buyers with high accuracy. The user's device type (Laptop or Mobile) influences purchase behavior, so separate models were developed for each segment.

## Key Features

- 📊 **Data Preprocessing**: Handling missing values, encoding categorical features, scaling numerical data.
- 🔍 **Exploratory Data Analysis**: Visual insights into user behavior and its relation to purchase propensity.
- 🧠 **Machine Learning Models**: Binary classification models using XGBoost, optimized separately for laptop and mobile users.
- 📈 **Evaluation**: Confusion matrix, classification report, ROC curve, and AUC score for thorough performance assessment.
- 💾 **Model Persistence**: Trained models and scalers saved as `.pkl` files for easy deployment.
- 🔁 **Prediction Utility**: Modular function to predict ticket purchase probability for new user inputs.

## Technologies Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Pickle

## Folder Structure

```
📁 propensity-modeling/
├── travel_data.csv
├── propensity_modeling.ipynb
├── laptop_model.pkl
├── mobile_model.pkl
├── laptop_scaler.pkl
├── mobile_scaler.pkl
├── README.md
```

## Usage

1. Place your dataset as `travel_data.csv` in the project directory.
2. Run the notebook `propensity_modeling.ipynb` to preprocess data, train models, and generate evaluations.
3. Use the `predict_ticket_purchase()` function with user input and device type to infer purchase likelihood.

## Example Inference

```python
example_input = {
    'Yearly_avg_view_on_travel_page': 20,
    'total_likes_on_outstation_checkin_given': 5,
    ...
}
predict_ticket_purchase(example_input, device_type='Laptop')
```

## Outcome

The model allows the client to run **cost-effective digital ad campaigns** by targeting only high-probability users, reducing marketing overhead while improving conversion rates.

## Author

Mekanapriya 
Python Developer  
© 2025 All Rights Reserved
