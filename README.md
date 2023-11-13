# Feature-Selection
## General Purpose
Quantify Dependency of Features (X) and Target (Y). Primarily used for classification problems (with Discrete Y). May be extend to regression problems (Continuous Y).
//May be used for: 1) Univariate feature selection; 2) Visualize dependency between Y and Top informative features.


## Commonly Used Feature selection Methods: 
Typically there are three types of methods: 
 - Wrapper (which train model iteratively and gradually exclude unimportant features)
 - Embedding (the feature selection are included in model training process, such as Lasso, Ridge, etc)
 - Filter (assign score metrics for each feature with the help of various statistical calculations and then filter out the most irrelevant ones)
### Variance Threshold
Simply remove low variance features (for variance indicates information)
### Mutual_info_classif
Using mutual information to measure depency of two variables (not limit to linear relationship)
### F_classif
It uses the ANOVA f-test for the features and takes into consideration only linear dependency
### SelectKBest
A more general method that can include other methods
### Pearson Correlation
assesses linear relationships
### Spearmon Correlation
evaluates monotonic relationships

reference:
 - https://medium.com/@hertan06/which-features-to-use-in-your-model-350630a1e31c
 - https://zhuanlan.zhihu.com/p/99776961
