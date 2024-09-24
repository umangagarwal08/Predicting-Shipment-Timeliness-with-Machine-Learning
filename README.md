# E-commerce Customer Shipment Analytics

## Project Overview

This project explores customer and shipment data from an international e-commerce company that specializes in selling electronic products. The goal is to predict whether a product will be delivered on time, based on various customer and shipment-related features. By using advanced machine learning techniques and multiple classification models, we aim to uncover key insights that can help improve customer service and streamline logistics.

## Dataset Information

The dataset consists of 10,999 records and 12 variables related to customer behavior, shipment details, and delivery status. The variables are:

- **ID**: Unique identifier for each customer.
- **Warehouse Block**: Warehouse division (A, B, C, D, E).
- **Mode of Shipment**: Shipping method (Ship, Flight, Road).
- **Customer Care Calls**: Number of calls made to customer care regarding the shipment.
- **Customer Rating**: Rating given by customers (1 to 5).
- **Cost of the Product**: Product cost in US dollars.
- **Prior Purchases**: Number of prior purchases made by the customer.
- **Product Importance**: Importance level of the product (Low, Medium, High).
- **Gender**: Gender of the customer (Male, Female).
- **Discount Offered**: Discount offered on the product.
- **Weight in gms**: Weight of the product in grams.
- **Reached on Time**: Target variable. 1 indicates the product did NOT reach on time, 0 indicates the product reached on time.

## Project Objectives

- **Predict whether a product will be delivered on time** based on various factors.
- **Analyze customer behavior** and its impact on delivery times.
- Use **classification models** to make accurate predictions.

## Models Used

To predict the target variable (whether the product reached on time), we used various classification models, including:

1. **Logistic Regression**
2. **Naive Bayes**
3. **Random Forest**
4. **Decision Tree**
5. **Ada Boost Classifier**
6. **XGB Classifier**
7. **Voting Classifier**
8. **Stacking Classifier**
9. **Gradient Boosting Classifier** (final model)

### Model Tuning

To enhance model performance, **GridSearchCV** was used for hyperparameter tuning across all models. This helped identify the best combination of parameters for each model.

### Final Model: Gradient Boosting Classifier

The **Gradient Boosting Classifier** provided the best performance after fine-tuning with **GridSearchCV**.

- **Accuracy**: 68%
- **Precision**: 93%
- **F1 Score**: 67%
- **Cohen's Kappa Score**: 40%

## Evaluation Metrics

- **Accuracy**: Measures the overall correctness of the model.
- **Precision**: Indicates the proportion of positive predictions that were actually correct.
- **F1 Score**: Harmonic mean of precision and recall, balancing the two.
- **Cohen’s Kappa**: Measures inter-rater agreement, accounting for chance.

## Tools and Libraries Used

- **Python**
- **Pandas**: Data manipulation and preprocessing
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning models and GridSearchCV for fine-tuning
- **Gradient Boosting Classifier**: Final model for classification

## Conclusion

This project demonstrated the effectiveness of machine learning techniques in predicting product delivery times based on various customer and shipment factors. The **Gradient Boosting Classifier** provided solid predictive performance with 68% accuracy and 93% precision, making it a useful model for improving logistics and customer satisfaction.

## Future Work

- Explore additional features or external data sources to improve model performance.
- Implement additional boosting methods like XGBoost or CatBoost for comparison.
- Enhance feature engineering to capture more complex relationships in the data.

---

## Acknowledgements

I would like to acknowledge the data collected and made available for this project through Kaggle. This project has been uploaded to my GitHub repository for reference.

