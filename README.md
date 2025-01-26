# Loan Default and Price Prediction Project

This project comprises two interconnected objectives, each represented by a separate Jupyter Notebook. Both objectives aim to apply machine learning methodologies to solve practical problems in predictive analytics. Below is a detailed overview of the project's objectives, methodologies, and other essential information.

---

### Project Structure
1. **Loan Default Prediction Notebook:** Contains steps for predicting loan defaults.
2. **Price Predictor Notebook:** Contains steps for predicting prices.

---

## Objective 1: Loan Default Prediction

### Overview
This notebook focuses on predicting the likelihood of loan defaults using historical data. It aims to help financial institutions make informed decisions about lending by identifying potential risks.

### Methodology
1. **Importing Packages:**
   - Essential Python libraries such as pandas, NumPy, and machine learning frameworks are imported.

2. **Data Import and Exploration:**
   - Loan-related datasets are loaded and inspected for structure, completeness, and initial insights.

3. **Data Visualization:**
   - Visual techniques (e.g., scatterplots and barplots) are used to understand trends and relationships in the data.
  
     ![Image](https://github.com/user-attachments/assets/2ea80257-93ba-4dbc-81e2-f7fe2bfdf705)

4. **Model Preparation:**
   - Data preprocessing steps include handling missing values, feature selection, and encoding categorical variables.

5. **Model Initialization:**
   - Machine learning model (Random Forest Classifier) is initialized and prepared for training.

6. **Training and Evaluation:**
   - Models are trained, and performance metrics such as accuracy, precision, recall, f1 score and roc-auc are computed
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
    <td>Random Forest CLassifier</td>
    <td align="center">99.0%</td>
    <td align="center">96.0%</td>
    <td align="center">98.0%</td>
    <td align="center">97.0%</td>
    <td align="center">99.0%</td>
  </tr>
</table>

   -  A confusion matrix, ROC-AUC and Calibration Curves were used to visualize the model's performance.

![8 1](https://github.com/user-attachments/assets/09c06986-6992-4558-aee6-58905a93bfc1)


7. **Loan Default Predictor:**
   - The final model is fine-tuned and deployed for predicting loan defaults.

---

## Objective 2: Price Prediction

### Overview
This notebook aims to predict the prices of items or services based on various features. It can be applied to domains such as real estate, retail, and e-commerce.

### Methodology
1. **Importing Packages:**
   - Relevant Python libraries for data manipulation and visualization are imported.

2. **Data Import and Exploration:**
   - The dataset is loaded, and exploratory data analysis (EDA) is performed to gain insights.

3. **Feature Engineering:**
   - New features are created, and existing features are transformed to enhance predictive power.

4. **Data Visualization:**
   - A lineplot was created to better understand data.
  
     ![Image](https://github.com/user-attachments/assets/216051a0-fa28-43c8-b152-6136abc23793)

5. **Model Preparation:**
   - Data is preprocessed, including normalization, handling outliers, and splitting into training/testing sets.

6. **Training and Evaluation:**
   - Machine learning models such as linear regression and random forest regressor are trained.


   - Regression plots are used to visualize their performance
  
     ![Image](https://github.com/user-attachments/assets/da7eef4f-ef60-4238-9046-ffad1ea9c150)

7. **Price Prediction Logic:**
   - Models are trained to predict prices, and results are evaluated using metrics like MAE MAPE and R-squared.

<table align="center">
 <tr>
    <th>MODEL</th>
    <th>MAE</th>
    <th>MAPE</th>
    <th>R²</th>
 </tr>
 <tr>
    <td>Random Forest Regressor</td>
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


8. **Price Predictor:**
   - The finalized model is used for price prediction on new data.
