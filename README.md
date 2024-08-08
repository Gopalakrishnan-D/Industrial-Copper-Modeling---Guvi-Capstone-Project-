

**Project Title:**
Industrial Copper Modeling

**Skills Gained:**
Python scripting, Data Preprocessing, Exploratory Data Analysis (EDA), Streamlit

**Domain:**
Manufacturing

**Problem Statement:**
The copper industry often faces challenges with sales and pricing data, including skewness and noisy data that impact manual predictions. These issues can be time-consuming and may not yield optimal pricing decisions. A machine learning regression model can enhance accuracy by employing techniques such as data normalization, feature scaling, and outlier detection, using algorithms resilient to skewed and noisy data. Additionally, lead classification can be improved using a model that evaluates and classifies leads based on their likelihood of becoming a customer, focusing on statuses like "WON" for success and "LOST" for failure.

**Solution Approach:**

1. **Data Exploration:**
   - Identify and address skewness and outliers in the dataset.
   - Transform and clean data, including converting invalid entries in `material_ref` to null.

2. **Data Preprocessing:**
   - Handle missing values with mean/median/mode imputation.
   - Address outliers using techniques like IQR or Isolation Forest.
   - Treat skewness with transformations (e.g., log, Box-Cox).
   - Encode categorical variables using suitable techniques (e.g., one-hot, label encoding).

3. **Exploratory Data Analysis (EDA):**
   - Visualize data to understand outliers and skewness before and after treatment using Seaborn plots (boxplot, distplot, violinplot).

4. **Feature Engineering:**
   - Create new features or aggregate existing ones as needed.
   - Remove highly correlated columns using a heatmap.

5. **Model Building and Evaluation:**
   - Split data into training and testing sets.
   - Train and evaluate classification models (e.g., ExtraTreesClassifier, XGBClassifier) and regression models.
   - Optimize models using cross-validation and grid search.
   - Interpret and assess model performance.

6. **Model Deployment with Streamlit:**
   - Develop an interactive web page allowing users to input data and obtain predictions for both regression (Selling_Price) and classification (Status: WON/LOST).
   - Apply the same preprocessing and feature engineering used during model training.

**Data Overview:**
- `id`: Unique transaction/item identifier.
- `item_date`: Date of transaction/item record.
- `quantity tons`: Quantity in tons.
- `customer`: Customer identifier.
- `country`: Country associated with the customer.
- `status`: Current transaction status.
- `item type`: Category of items.
- `application`: Specific use/application of items.
- `thickness`: Thickness of items.
- `width`: Width of items.
- `material_ref`: Material reference/identifier.
- `product_ref`: Product reference/identifier.
- `delivery date`: Expected/actual delivery date.
- `selling_price`: Price at which items are sold.

**Learning Outcomes:**
- Master Python programming and libraries like Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, and Streamlit.
- Gain experience in data preprocessing, including handling missing values, outlier detection, and normalization.
- Develop skills in EDA techniques for data visualization.
- Learn and apply machine learning techniques for regression and classification tasks.
- Build and optimize machine learning models and use evaluation metrics.
- Create a Streamlit web application for interactive model predictions.
- Understand and address challenges in the manufacturing domain using machine learning.