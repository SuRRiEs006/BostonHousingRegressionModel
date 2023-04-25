


# Boston Housing Dataset Analysis
### Why did I choose to take on this project?

My business elective (big data in business and finance) assignment asked us to discuss the potential for big data in business and the opportunities as a result of new technologies. I decided to go hands-on with the assignment and learn the basics of machine learning algorithms. 




### TLDR;
This project focuses on the analysis of the Boston Housing dataset using Python, Jupyter Notebook, and various data analysis and machine learning libraries. The dataset contains information on the housing market in Boston, such as the average number of rooms per dwelling, the percentage of lower status of the population, the pupil-teacher ratio by town, and the median value of owner-occupied homes.
After a lot of research, I decided on the Random Forest Regressor model.
- I cleaned the Boston housing dataset
- Made a correlation heat map to better understand the underlying correlations. 
- After a lot of research, I decided on the Random Forest Regressor model.
- Took the train data and fit it to a random forest regressor model
    - With some parameter tuning, I improved the model's success rate from 79% to 84%.

## Table of Contents

- [Project Overview](#project-overview)
- [Libraries Used](#libraries-used)
- [Data Preprocessing](#data-preprocessing)
- [Data Visualization](#data-visualization)
- [Model Training and Evaluation](#model-training-and-evaluation)

## Project Overview

The main goal of this project is to analyze and understand the relationships between various features in the Boston Housing dataset and predict the median value of owner-occupied homes using machine learning models.

## Libraries Used

- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-Learn

## Data Preprocessing

The dataset is loaded into a Pandas DataFrame, and the following preprocessing steps are performed:

1. Histograms of the dataset's features are plotted for initial visualization.
2. The dataset's information is printed to the console to ensure proper data types and non-null counts.
3. The `MEDV` (median value) and `LSTAT` (% lower status) features are square-root transformed for better distribution and to reduce skewness.
4. Histograms of the transformed features are plotted for comparison.

## Data Visualization

Several visualizations are generated to explore the relationships between the dataset's features:

1. A heatmap of the feature correlations is plotted using Seaborn.
2. A scatterplot of `LSTAT` vs. `RM` (average number of rooms per dwelling) is created, with data points colored according to the `MEDV` value.
3. A scatterplot of `LSTAT` vs. `MEDV` is generated to visualize the relationship between these two features.

## Model Training and Evaluation

The dataset is split into training and testing sets, with features `LSTAT`, `RM`, and `PTRATIO` (pupil-teacher ratio) as predictors and `MEDV` as the target variable. A Random Forest Regressor model is trained on the training set and evaluated on the testing set, achieving an R^2 score of 0.8439, indicating that the model explains approximately 84.39% of the variance in the target variable.
