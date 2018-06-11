---
layout: post
title: "Systematized Predictive Modeling"
date: 2015-06-03
categories: machinelearning
---

_Preprocessing_
1. Zero mean (subtract the mean from each predictor) to center the data.
2. Divide by standard deviation to scale the data.
3. DateTime
4. One-Hot Code
5. Look For skewness, log/sqrt/Box Cox transform if necessary (Boxcox)
6. Resolve Outliers (and understand their meaning) (apply spatial sign if model is sensitive to outliers)
7. Eliminate Missing Data (Can be problematic if missingness is predictive. Tree Based Models can deal with missing data)
8. Imputation/Interpolation (KNN or intermediate regression model)

___
<br>

_Exploratory Data Analysis_
1. Maximal Information Coefficient Matrix / Correlation Matrix
2. Box-Chart Everything
3. Scatter Every Combination of Features
4. Pivot Tables
5. Group by particular features
6. Histogram Everything
7. Outlier Analysis
8. Transform Variables (Square, Cube, Inverse, Log) and Plot
9. Summary (Mean, Mode, Minimum, Maximum, Upper/Lower Quartiles, Identify Outliers)

___
<br>

_Data Reduction_
1. Principal Component Analysis 
2.Linear Discriminant Analysis (For Classification)
3. Feature Selection (Only use the components that account for a majority of the information when Modeling
4. Remove Low/Zero Variance Predictors
5. Remove multicollinear heavily correlated features
6. Isomap
7. Lasso

___
<br>


_Algorithms for Regression_
1. Linear Regression
	- Ridge Regression / Lasso / Elastic Net 
	- Best Subset Selection 
	- Forward and Backward Stepwise, Stagewise
2. Partial Least Squares
3. Principal Components Regression
4. Neural Networks
	- CNN
	- RNN
		-LSTM
5. Multivariate Adaptive Regression Splines
6. Support Vector Regressor
7. K-Nearest Neighbors
8. Regression Decision Trees
9. Bagged Trees
10. Random Forests
11. Extremely Random Forests
12. Gradient Boosted Trees
13. Generalized Linear Model
14. Generalized Additive Model

___
<br>


_Evaluating Regression_
1. RMSE
2. MAE
3. Median
4. R2
5. Visualization

___
<br>


_Algorithms for Classification_
1. Logistic Regression
	- L1, L2, Elastic Net
2. Discriminant Analysis
3. Linear Discriminant Analysis
4. Quadratic Discriminant Analysis
5. Neural Networks
	- CNN
	- RNN
		- LSTM
6. Support Vector Classifier
7. K-Nearest Neighbors
8. Naive Bayes
9. Classification Trees
10. Bagged Trees
11. Random Forests
12. Extremely Random Forests
13. Gradient Boosted Trees
14. Generalized Additive Model

___
<br>


_Evaluating Classification_
1. ROC Curve
2. Confusion Matrix
3. F1 Score
4. Heat Map
5. Overall accuracy rate
6. Kappa Statistic
7. Sensitivity
8. Specificity
9. AUC 

___
<br>


_Unsupervised Learning_
1. K-Means
	- K-Means++
	- K-Medoids
2. Hierarchical Agglomerative Clustering
	- Single Linkage, Complete Linkage, Average Linkage, Centroid Criterion
3. Principal Components Analysis
4. Spectral Clustering
5. Affinity Propagation
6. Biclustering
7. Gaussian Mixture Model

___
<br>


_Classification Class Imbalance_
1. Model Tuning (Tune Parameters For Sensitivity)
2. Alternate Cutoffs (Using ROC Curve)
3. Adjusting Prior Probability
4. Unequal Case Weights
5. Down Sampling
6. Up Sampling
7. Alter Cost Function
8. Dynamic Structure (Cascade of classifiers)

___
<br>


_Feature Evaluation_
1. Coefficients in Linear Models
2. Random Forest Importances (variance for regression, information gain for classification)
3. Pearson Correlation with Outcome
4. Maximal Information Coefficient (MIC)
5. Distance Correlation (code)
6. Model with/without feature
7. Randomly shuffle the feature between data points, check difference in model quality
8. Lasso Automatic Selection
9. Mean Decrease Accuracy (code)
10. Stability Selection
11. Recursive Feature Elimination

___
<br>


_Parameter Tuning_
1. Cross Validation
2. Bootstrap
3. Grid Search (ex)

___
<br>



_Text Features_
1. n-Grams
2. Word Vector Representations (Word 2 Vec)
3. Bag of words
4. Word counts
5. Lengths
6. Tf-idf
7. Term frequency, weighted by its rarity
8. topic modeling (LDA)

___
<br>


_Modeling Techniques_
1. Feature Engineering
	- Basis Expansions
	- Combine Features
	- average values, median values, variances, sums, differences, maximums or minimums, and counts.
2. Stacking (using output of one algorithm as input to the next)
3. Internal Prediction
4. Blending (Especially with differentiated models)
5. Account For Missing Data (It can be information)
6. External Data
7. Acquire Domain Knowledge for Feature Engineering
8. Random Forest, Boosters, Trees Importances for Feature Exploration
9. Clustering for feature creation
10. Distance to Class Centroid
