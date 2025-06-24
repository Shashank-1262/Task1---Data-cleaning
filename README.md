# **Task 1 Data Cleaning and Preprocessing**

1. **Imported Libraries**:
Data processing, visualization, and scaling were done with the use of 'pandas', 'numpy', 'seaborn', 'matplotlib', and 'scikit-learn'.

2. **Loaded Dataset**:
Imported and read the Titanic dataset using 'pd.read_csv()' and printed the basic metadata, descriptive statistics and missing values.

3. Missing Data managed:

Replaced missing 'Age' with 'median'.
* Added 'Unknown' in the missing entries of 'Cabin'.
These 'Embarked' cells were filled in with the 'mode'.

4. **Unnecessary Columns that had been dropped**:
Dropped PassengerId, Name and Ticket because they are not important to model.

5. **Encoded Categorical**:

Applied 'LabelEncoder' transformation on the 'Sex' feature to a numerical value.
Applied 'get_dummies()' to 'Embarked' and present 'drop_first=True' in order to avoid dummy variable trap.

6. **Visualized Outliers**:
Developed a box plot that shows the existence of possible outliers in Age column and Fare column.

7. **Removed Outliers**:
Determined and applied a function with the help of 'IQR method' to drop outliers in 'Age' and 'Fare'.

8. The **scaled numerical features** are the features that provide scales to numerical values.
Applied 'StandardScaler' to 'Age' and 'Fare', to make them have
a mean of 0 and standard deviation of 1.

10. Printed Final output:
Shown the cleaned, transformed and scaled data using '.head()', '.describe()'.
