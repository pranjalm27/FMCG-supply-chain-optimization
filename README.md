# FMCG-supply-chain-optimization

### Project Summary 
This project focuses on optimizing the supply chain management of an FMCG company that has entered the instant noodles market. The primary challenge addressed is the mismatch between demand and supply across various warehouses, which has been leading to inventory losses and inefficiencies.

#### Objective:
To build a machine learning model that predicts the optimal weight of products to be shipped from each warehouse, thereby reducing inventory costs and improving supply chain efficiency.

#### Approach:
1. **Data Collection & Preprocessing**: Historical data related to product weight, storage issues, transportation problems, and other relevant features were collected and cleaned for analysis.

2. **Exploratory Data Analysis (EDA)**: Initial analysis was performed to understand the data distribution, correlations, and potential outliers. A significant positive correlation was identified between product weight and storage issues reported.

3. **Feature Selection**: Using feature importance techniques, the most significant features affecting the dependent variable (product weight) were selected. The top feature, `storage_issue_reported_l3m`, showed a high correlation with the dependent variable.

4. **Model Building**: Several regression models were trained, including Gradient Boosting, Random Forest, Bagging, and AdaBoost. Gradient Boosting was identified as the best-performing model.

5. **Model Evaluation**: The models were evaluated based on Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R^2) scores. The Gradient Boosting model achieved the highest R^2 score of 0.99, indicating strong predictive power.

6. **Optimization & Deployment**: The final model was fine-tuned and can be used to predict the optimal shipping weight from each warehouse, helping to align supply with demand.

#### Results:
- The Gradient Boosting model provided the best performance, with an MSE of 822,763.55 and an R^2 score of 0.99, indicating a highly accurate prediction of product weight for shipping.

#### Key Insights:
- A very high importance score (98.87%) was observed for the storage_issue_reported_l3m feature, indicating a strong relationship between storage issues and product weight, which suggests that addressing storage conditions could optimize supply efficiency.
-  The approved_wh_govt_certificate feature also played a crucial role, with an importance score of 0.87%, suggesting that warehouses with government certification had a significant impact on predicting product weight, likely due to their better storage practices.
- The analysis pointed to specific areas for operational improvement, such as better managing storage conditions and ensuring regulatory compliance, which can lead to more accurate demand forecasting and optimized supply chain processes.

#### Conclusion:
This project successfully developed a machine learning solution that optimizes the supply chain process, reducing losses due to inventory mismanagement and improving overall operational efficiency for the FMCG company.

#### Future Work:
- Further fine-tuning of the model with additional features or external factors such as market trends.
- Implementation of real-time data monitoring to continuously improve the model’s predictions.
