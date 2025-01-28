Tool used- Python
Libraries:
NumPy: For numerical operations and array manipulations.
Pandas: For data manipulation and handling.
Matplotlib: For plotting and visualizing data.
Seaborn: For statistical data visualization built on top of Matplotlib.
PCA (Principal Component Analysis): For dimensionality reduction.
RandomForestClassifier: A machine learning model for classification tasks.
LogisticRegression: A machine learning model for binary/multi-class classification.
train_test_split: To split the dataset into training and test sets.
classification_report, accuracy_score: For evaluating model performance with metrics such as precision, recall, F1-score, and accuracy.
StandardScaler: For standardizing features by removing the mean and scaling to unit variance.
GridSearchCV: For hyperparameter tuning by exhaustively searching through a grid of parameters.

Objective- The objective of this analysis is to apply exploratory data analysis (EDA) techniques to identify key factors contributing to loan defaults within the banking and financial services industry. By examining a dataset that includes borrower demographics, financial history, and loan details, we aim to uncover patterns and correlations that can enhance risk assessment and decision-making processes. The ultimate goal is to generate actionable insights that financial institutions can use to optimize their lending strategies, reduce the risk of defaults, and improve overall profitability.
Provided Datasets
1. Application_data.csv: It contains all the information of the client at the time of application. The data is about whether a client has payment difficulties.
2. Previous_application.csv: It contains information about the client’s previous loan data. It contains the data whether the previous application had been Approved, Cancelled, Refused or Unused offer.

Task1 - EDA 
In the Exploratory Data Analysis (EDA) the primary goal is to understand the dataset, uncover patterns, spot anomalies, and check assumptions before moving on to more complex modeling. 
Data Loading and Overview:
The dataset is loaded using Pandas (e.g., pd.read_csv() for CSV files). We inspect the dataset using methods like head(), info(), and describe() to understand its structure, types of data, and basic summary statistics.
Handling Missing Data:
We identify missing values using methods like isnull() or isna(), and handle them by either dropping or imputing the missing data based on the context.
Data Cleaning:
We clean the data by removing duplicates, correcting data types (e.g., converting strings to datetime), and fixing any inconsistencies or errors.
Univariate Analysis:
For individual features, we use histograms, box plots, and count plots to visualize the distribution of the data and identify any skewness, outliers, or patterns in each feature.
Bivariate Analysis:
We explore relationships between two variables using scatter plots, pair plots, or correlation matrices. For categorical data, we use cross-tabulations or bar plots to check the relationship between categorical features.
Multivariate Analysis:
When dealing with multiple variables, we can use heatmaps, pair plots, or dimensionality reduction techniques like PCA to visualize interactions between multiple features.
Visualization:
Matplotlib and Seaborn are often used to create plots that provide visual insights, helping to understand trends, distributions, and correlations more intuitively.

Task2- Predictive modelling
The goal of predictive model is to build a range of models to compare performance, identify strengths, and determine the most effective approach for predicting loan defaults.
Model building steps include: Data Processing, Feature Engineering, Dimensionality Reduction, Handling Imbalance Data, Algorithm Selection
Models Prepared:
Model 1: Random Forest Classifier (Initial Model)
Model 2: Random Forest Classifier +Domain Knowledge
Model 3: Random Forest +Correlated features
Model 4: Random Forest with Grid Search Optimization
Model 5: Random Forest + PCA
Model 6: Logistic Regression + PCA
Conclusion:
Out of all the 6 models Model 6 is the most reliable for risk analytics, crucial for minimizing missed defaulters while balancing precision and recall.
Model 6 came out to have highest accuracy (66.55%) and F1 score (0.68); best for identifying defaulters with a good balance between precision and recall.




