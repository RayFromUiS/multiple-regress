This is working flow for multiple regerssion,it includes

- deal with missing value
- outerlier detection
- EDA
- modeling building
- model tuning

with recrusive featuring engineering


# initial model could be considered as a base model, it working flow does the follows
1drop the missing values with more than 10%;
2using IQR for outlier detection("price")
3then using sklearn SimpleImputer to impute the missing value for categorical value and numerical columns
4feature enginering is applied on different dimensions,introduce "facilities life" as new dimension, then using mlxtend forward selection
choose the most evident features
5finall sklearn Pipeline is bulid for the processed data, sklearn.ColumnTransform is used for scaling and encoding the corresponding
data types
6Model is selected based on a grid search with defferent estimator,
7temporialy Lasso give the best performance, r2_scroe is 0.91


# second stage it mainly focused on outlier detection,with other steps maintained
