# House price prediction

This project is just a very basic attempt of classification of data with numerous features, which means, amongst other, dealing with high dimensionality.

Additionally, it is a good opportunity to learn some scikit-learn functionalities.

What has been done?
* Attempt 1: Extracting (approximately) the numeric features best explaining the data and "fine-tuning" few parameters of the model; although both done rather primitively to be frank.
* Attempt 2: Imputing the missing data and encoding the categorical features using One-Hot encoding and label encoding (via sklearn tools).
* Attempt 3: Mostly the same as previously, but `Pipeline` and `ColumnTransformer` functionalities are used.