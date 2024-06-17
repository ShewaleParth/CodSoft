# Titanic Survival Prediction

This project is a Jupyter Notebook that performs data analysis and machine learning on the Titanic dataset to predict whether a passenger survived the sinking of the Titanic.

## Dependencies

The following libraries are used in this project:

- `numpy`
- `pandas`
- `matplotlib.pyplot`
- `seaborn`
- `sklearn.model_selection`
- `sklearn.linear_model`
- `sklearn.metrics`
- `sklearn.impute`

## Data Collection and Processing

1. The Titanic dataset is loaded from a CSV file using `pandas`.
2. The first five rows of the dataset are displayed, and the number of rows and columns is checked.
3. The data types and missing values are inspected.
4. Missing values in the `Age` and `Embarked` columns are handled by replacing them with the mean age and the most frequent value, respectively.
5. The `Cabin` column is dropped due to a large number of missing values.

## Data Analysis and Visualization

1. Statistical measures of the dataset are obtained using `describe()`.
2. The number of survivors and non-survivors is counted using `value_counts()`.
3. Various count plots are created using `seaborn` to visualize the distribution of variables such as `Survived`, `Sex`, `Pclass`, and `SibSp`.
4. The number of survivors by gender is also visualized.

## Encoding Categories

The `Sex` and `Embarked` columns are encoded as numerical values using dictionaries.

## Separating Features and Target

The dataset is split into features (`X`) and the target variable (`Y`), which is the `Survived` column.

## Splitting Data into Training and Test Sets

The data is split into training and test sets using `train_test_split()` with a test size of 0.2.

## Model Training and Evaluation

1. A logistic regression model is trained on the training data using `LogisticRegression()`.
2. The accuracy of the model on the training and test data is calculated using `accuracy_score()`.

## Conclusion

This Jupyter Notebook provides a comprehensive analysis of the Titanic dataset, including data preprocessing, visualization, and machine learning model evaluation. The logistic regression model achieves a reasonable accuracy on the test data, demonstrating its ability to predict passenger survival on the Titanic.
