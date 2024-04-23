# **Boat Prices Prediction Study** :speedboat:

## *What is it?*

This project aimed to create regression models for predicting the prices of boats, utilizing some features. The dataset, which contains numerical and categorical columns, was obtained from the Kaggle website, in the Mexwell profile [1]. The processes performed in this study are listed above:

- Missing values deletion
- Exploratory Data Analysis (EDA) with numerical variables, using distribuition plots, such as box-plots and violin plots
- Outliers remotion
- Numerical and categorical features ranking creation, using $\phi_k$ correlation with the target variable, 'price'
- Linear models creation, by adding numerical features, one by one, to be executed in a cross-validation process
- Random Forest models creation, by adding numerical features, also one by one, to be executed in a cross-validation process
- $R^2$ and MSE (Mean Squared Error) observation

During the study, was observed that the Random Forest models using numerical and categorical features got tiny better results than when just taking the numerical features:

| Model | MSE (average) | $R^2$ | Number of features |
| --- | --- | --- | --- |
| Random Forest with numerical features | 0.115803 | 0.9007 | 7 |
| Random Forest with numerical and categorical features | 0.109965 | 0.907 | 10 |

Although, the models with categorical features brought more complexity than when just working with numerical features.

## *Tools used* :hammer:
The complete list of Python libraries used is:
- Scikit-Learn
- Pandas
- NumPy
- phik
- Seaborn
- Matplotlib
- tqdm

They all can be installed with the installers available in the 'INSTALL' folder, or using the pip install command.

## *References* :earth_americas:

[1] https://www.kaggle.com/datasets/mexwell/boat-price-prediction