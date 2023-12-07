# Customer Churn Prediction

### Introduction

In this project, we employ a Random Forest predictive model to analyze and predict customer churn for a company. The analysis is conducted using R programming language, focusing on understanding the factors contributing to customer churn and predicting future trends.

### Methodology

1. **Data Loading and Preparation**: The dataset 'WA_Fn-UseC_-Telco-Customer-Churn.csv' was loaded into R. Necessary data cleaning steps were performed, including handling missing values and data type conversions.

2. **Library Imports**: Various R libraries were imported to aid in data manipulation, visualization, and modeling. Notable libraries include `dplyr`, `ggplot2`, `tidyr`, `corrplot`, `tidyverse`, `caret`, and `randomForest`.

3. **Data Exploration**: 
   - The dataset's structure was examined using `str()` and `skim()`.
   - Unique values for categorical variables were identified.
   - Gender distribution and churn distribution were visualized using bar plots.
   - The difference and percentage difference between churned and non-churned customers were calculated and displayed.
   - A histogram was created to observe the distribution of monthly charges.
   - A heatmap was generated to visualize correlations between selected numerical features.

4. **Predictive Modeling - Random Forest**:
   - The 'Churn' variable was converted to a factor for modeling purposes.
   - The dataset was split into training and testing sets using a 70-30 split.
   - Predictors and the target variable were defined.
   - A Random Forest model was trained on the training set.
   - Predictions were made on the test set using the trained model.

5. **Model Evaluation**:
   - A confusion matrix was created to assess the model's performance.
   - Accuracy and recall metrics were calculated and displayed.

### Key Findings and Analysis

- **Gender and Churn Distribution**: Initial analysis showed the distribution of customers by gender and their churn status, providing insights into potential trends in customer behavior.
![image](https://github.com/zashari/DS_CustomerChurn/assets/63639442/f35ffb59-2110-472f-b999-51b3bf1e613d)


- **Active vs Non-Active Customers**: The analysis revealed a significant percentage difference between active and non-active customers, indicating the extent of churn in the customer base.
![image](https://github.com/zashari/DS_CustomerChurn/assets/63639442/e2ea493d-187b-479b-a0d8-a0a1bd93621c)
```Percentage difference of churn: 63.80012 %```

- **Monthly Charges Distribution**: The histogram of monthly charges might provide insights into customer segments more likely to churn.
![image](https://github.com/zashari/DS_CustomerChurn/assets/63639442/421fd28b-93f2-4f28-9c2c-f3ff0f0a7100)


- **Correlation Analysis**: The heatmap highlighted key relationships among features like tenure, monthly charges, and total charges, which could be pivotal in understanding factors influencing churn.
![image](https://github.com/zashari/DS_CustomerChurn/assets/63639442/57010970-c7d9-4148-9385-0309c246d96b)

- **Model Performance**: 
   - The Random Forest model's performance was evaluated using accuracy and recall metrics.
   - The confusion matrix provided a detailed view of the model's ability to correctly predict churn.
    ```
    predictions   No  Yes
            No  1393  256
            Yes  155  304

    Accuracy: 80.5%
    Recall: 66.23%
    ```
### Conclusion

The predictive analysis using a Random Forest model provided valuable insights into customer churn. The model's performance, gauged by accuracy and recall, demonstrates its effectiveness in predicting churn. Understanding these patterns can help the company devise targeted strategies to reduce customer churn and improve retention. The detailed data exploration and visualization steps also shed light on the characteristics of the customer base, contributing to more informed decision-making. 

### Future Work

- Further tuning of the Random Forest model could be explored to enhance its predictive performance.
- Additional features could be incorporated into the model to see if they provide more insights into customer churn.
- Comparative analysis with other machine learning models could be conducted to find the best model for predicting customer churn.
