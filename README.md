# House Price Prediction Model
This is the ML model that uses XGBoost regression algorithm to predict the house prices listed for sale.

--- Databases and their usage
  -- Stage 1
    Dataset here has been taken from Kaggle. We have two main datasets that are the basis for our analysis.
    1) train.csv
    2) test.csv

    The above datasets are processed and transformed into various formats such as:
    1) train_clean.csv
    2) test_clean.csv
    This dataset has been cleaned and processed with no missing values.

  -- Stage 2
    After performing data cleaning this dataset has been converted into wide format using one-hot encoding.
    1) housing_data.csv - Combined database using train_clean.csv and test_clean.csv. This database is converted into wide database by one-hot encoding for all the categorical variables.
    2) train_wide.csv - This database is the subset of housing_data.csv and has been prepared from housing_data.csv
    3) test_wide.csv - This database is the subset of housing_data.csv and has been prepared from housing_data.csv
    Datasets train_wide.csv and test_wide.csv are used for ML modeling and prediction.

  -- Miscellaneous datasets
    Datasets that are being used for analysis:
    1) missing_values.csv - Column wise count of missing values for training dataset.
    2) missing_values_test.csv - Column wise count of missing values for test dataset.

--- Jupyter Notebooks
  1) House Price Data Cleaning.ipynb - This notebook is used to clean the datasets i.e. Stage 1 as explained above.
  2) House Price Data Preparation.ipynb - This notebook is used to convert long dataset into wide format using one-hot encoding.
  3) House Price Regression Notebook.ipynb - This notebook is used to create and do hyper-parameter tuning of the ML model. And then used to do the house-price prediction.
