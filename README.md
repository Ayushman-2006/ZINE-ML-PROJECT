# ZINE-ML-PROJECT

## Stage 0(cleaning the data)

### 1)Load the Dataset:

Replace "combined_UNSW_NB15.csv" with the file name of your combined dataset.
Use pd.read_csv() to load it into a pandas DataFrame.

Explore the Dataset:

**df.head()**: Displays the first 5 rows to understand the structure.

**df.info()**: Shows column names, data types, and missing values.

**df.describe()**: Provides statistical summaries for numerical columns.

### 2)Handle Missing Values:

Check for missing values with isnull().sum().
Fill missing values:
For categorical columns: Use the mode (most frequent value).
For numerical columns: Use the mean.

### 3)Encode Categorical Variables:

Identify categorical columns using select_dtypes(include=["object"]).
Apply one-hot encoding to convert them into numerical features, ensuring they can be processed by machine learning models.

### 4)Normalize Numerical Features:

Use MinMaxScaler to scale numerical features between 0 and 1 for better model performance.

### 5)Save the Preprocessed Dataset:

Save the cleaned and transformed dataset as a CSV file for use in the next stages.
