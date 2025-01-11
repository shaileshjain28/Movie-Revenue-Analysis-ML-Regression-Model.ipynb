# IMDb Movie Revenue Prediction

## Project Overview:
This project aims to predict the revenue of movies using various features like budget, genre, IMDb score, status, and more. The goal is to provide movie producers with insights into how well their upcoming movies might perform at the box office.

### Dataset:
- **Source**: Kaggle
- **Rows**: 10,178
- **Columns**: 12
- **Key Features**: `date_x`, `score`, `status`, `orig_lang`, `budget_x`, `revenue`, `country`

### Objective:
The objective is to predict the revenue of movies based on multiple features. By doing so, movie producers can get an idea of the potential profitability of upcoming projects.

### Data Preprocessing:
- **Missing Values**: No missing values, but duplicate rows were removed.
- **Outliers**: Outliers were handled using the Interquartile Range (IQR) method by filtering values above the upper whisker and below the lower whisker.
- **Feature Engineering**: Added new features, used **CountVectorizer** for feature extraction, and applied **Label Encoding** to categorical variables.
- **Unwanted Columns**: Removed irrelevant columns.

### Models Used:
To predict movie revenue, the following machine learning models were tested:
- **Linear Models**: Linear Regression, Lasso, Ridge, ElasticNet
- **Decision Trees**: Decision Tree Regressor
- **Ensemble Models**: Random Forest, AdaBoost, Gradient Boosting, XGBoost, LightGBM, CatBoost

### Key Results:
- Achieved **100% R-squared** with **CatBoost** and the lowest **RMSE**.
- **CatBoost** outperformed other models like Random Forest and LightGBM, providing the most accurate predictions.
- The model was trained using **K-Fold Cross Validation** with 10 folds to avoid overfitting.

### Tools and Libraries Used:
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, CatBoost, LightGBM
- **Techniques**: Feature Engineering, Label Encoding, Cross-validation

### Key Learnings:
- Gained hands-on experience in data cleaning, feature engineering, and model evaluation.
- Learned the importance of choosing the right models for high-dimensional data (e.g., CatBoost for large feature sets).
- Developed the ability to fine-tune models for high accuracy and low error rates.

### Conclusion:
This project helped me gain valuable skills in machine learning, especially in working with real-world datasets. It provided me with practical experience in predicting movie revenue, a useful tool for stakeholders in the film industry.

---

Feel free to check out the code and project files. Let me know if you have any questions or suggestions!
