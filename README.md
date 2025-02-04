# Loan Default and Price Prediction Project

This project comprises two interconnected objectives, each represented by a separate Jupyter Notebook. Both objectives aim to apply machine learning methodologies to solve practical problems in predictive analytics. Below is a detailed overview of the project's objectives, methodologies, and other essential information.

---

### Project Structure
1. **Loan Default Prediction Notebook:** Contains steps for predicting loan defaults.
2. **Price Predictor Notebook:** Contains steps for predicting prices.

---

## OBJECTIVE 1: Loan Default Prediction

This notebook focuses on predicting the likelihood of loan defaults using historical data. It aims to help financial institutions make informed decisions about lending by identifying potential risks.

## Methodology
### 1. **Importing Packages:**
   - Essential Python libraries such as pandas, NumPy, and machine learning frameworks are imported.

### 2. **Data Import and Exploration:**
   - Loan-related datasets are loaded and inspected for structure, completeness, and initial insights.

### 3. **Data Visualization:**
   - Visual techniques (e.g., scatterplots and barplots) are used to understand trends and relationships in the data.
  
     ![Image](https://github.com/user-attachments/assets/2ea80257-93ba-4dbc-81e2-f7fe2bfdf705)

### 4. **Model Preparation:**
   - Data preprocessing steps include handling missing values, feature selection, and encoding categorical variables.

### 5. **Model Initialization:**
   - Machine learning model (Random Forest Classifier) is initialized and prepared for training.

### 6. **Model Performance:**
 - **Exceptional Performance:**  
     - The Random Forest Classifier achieves outstanding performance across all metrics.

 - **Near-Perfect Accuracy:**  
     - The model achieves an impressive **accuracy of 99.0%.**

 - **Well-Balanced Precision and Recall:**  
     - The model has a **high precision (96.0%) and recall (98.0%)**, indicating that it is effective in both avoiding false positives and detecting true positives.

 - **Excellent F1 Score and ROC-AUC:**  
     - **The F1 score (97.0%) and ROC-AUC (99.0%)** confirm that the model has a **great balance between precision and recall** and is highly effective in distinguishing between classes. <p>

   <table align="center">
    <tr>
       <th>MODEL</th>
       <th>ACCURACY</th>
       <th>PRECISION</th>
       <th>RECALL</th>
       <th>F1 SCORE</th>
       <th>ROC-AUC</th>
    </tr>
    <tr>
       <td>Random Forest Classifier</td>
       <td align="center">99.0%</td>
       <td align="center">96.0%</td>
       <td align="center">98.0%</td>
       <td align="center">97.0%</td>
       <td align="center">99.0%</td>
    </tr>
   </table>

 -  **Confusion Matrix and  ROC-AUC and Calibration Curves**  
    - The Random Forest classifier demonstrates a **high level of accuracy** in predicting **both retained and churned customers**, **with minimal misclassifications.** 

    - **The ROC curve's AUC value of 99%** suggests the **model's exceptional performance** in distinguishing between retained and churned customers.

    - **The calibration curve** indicates that the predicted probabilities are **well-calibrated**, (The blue line closely follows the perfect calibration line (orange dashed line)) and accurately reflect the true likelihood of customer churn, making the model **reliable for predicting customer churn.**

    ![8 1](https://github.com/user-attachments/assets/09c06986-6992-4558-aee6-58905a93bfc1)

### 7. **Loan Default Predictor:**
   - The final model is fine-tuned and deployed for predicting loan defaults.

---

## OBJECTIVE 2: Price Prediction
This notebook aims to predict the prices of items or services based on various features. It can be applied to domains such as real estate, retail, and e-commerce.

## Methodology
### 1. **Importing Packages:**
   - Relevant Python libraries for data manipulation and visualization are imported.

### 2. **Data Import and Exploration:**
   - The dataset is loaded, and exploratory data analysis (EDA) is performed to gain insights.

### 3. **Feature Engineering:**
   - New features are created, and existing features are transformed to enhance predictive power.

### 4. **Data Visualization:**
   - A lineplot was created to better understand data.
  
     ![Image](https://github.com/user-attachments/assets/216051a0-fa28-43c8-b152-6136abc23793)

### 5. **Model Preparation:**
   - Data is preprocessed, including normalization, handling outliers, and splitting into training/testing sets.

### 6. **Model Performance**
 - Machine learning models such as linear regression and random forest regressor are trained.
 
 - **Regression Plot**    
    - **The Random Forest Regression model** appears to capture more complex patterns in the data, as indicated by the **tighter clustering** of data points around the regression line. 

    ![Image](https://github.com/user-attachments/assets/da7eef4f-ef60-4238-9046-ffad1ea9c150)
 
 - **Evaluation Metrics**
    - The Random Forest Regressor's better performance in terms of MAE and MAPE suggests that it is a more accurate and reliable model for predicting the target variable.

       - **Better Performance of Random Forest Regressor:**  
         The Random Forest Regressor outperforms Linear Regression in terms of MAE and MAPE.

       - **Lower MAE:**  
         The Random Forest Regressor has a lower MAE (0.2384) compared to Linear Regression (0.3123), indicating that it is better at predicting the target variable.

       - **Lower MAPE:**  
         The Random Forest Regressor also has a lower MAPE (0.0208) compared to Linear Regression (0.0273), indicating that it is better at predicting the target variable in terms of percentage error.
         
       - **Similar R²:**  
         Both models have the same R² value (0.8798), indicating that they explain the same amount of variance in the target variable.<p>

   <table align="center">
      <tr>
       <th>MODEL</th>
       <th>&emsp;&emsp;MAE&emsp;&emsp;</th>
       <th>&emsp;&emsp;MAPE&emsp;&emsp;</th>
       <th>&emsp;&emsp;R²&emsp;&emsp;</th>
    </tr>
    <tr>
       <td>Random Forest Regressor&emsp;&emsp;&emsp;&emsp;</td>
       <td align="center">0.2384</td>
       <td align="center">0.0208</td>
       <td align="center">0.8798</td>
    </tr>
    <tr>
       <td>Linear Regression</td>
       <td align="center">0.3123</td>
       <td align="center">0.0273</td>
       <td align="center">0.8798</td>
    </tr>
  </table>

### 7. **Price Prediction Logic:**
   - The finalized model is used for price prediction on new data.
