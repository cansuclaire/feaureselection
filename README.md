# feaureselection
www.patika.dev
            "Feature Selection"

*Univariate Selection

With statistical tests, strong relationships of independent variables with the dependent variable can be revealed.

For example, the significance scores of variables can be found with the chi-square test.

In addition, feature selection can be helped with Data Visualization.

*Feature Importance

Feature Importance scores are calculated.

*Correlation Matrix ve Heatmap

Important variables can be found using the correlation and heatmap.

*Feature Selection Methods

*Filter Methods
The filter method is performed at the data preprocessing stage.
![image](https://user-images.githubusercontent.com/97338597/186582854-e871563f-3c91-460e-ae1b-405899a2f526.png)


The following table shows the Filter methods according to Continuous and Discrete variables.
![image](https://user-images.githubusercontent.com/97338597/186582905-eb1bcfab-9a60-466c-a268-c1398a1d0810.png)


Correlation is used to Decipher the relationships between variables and each other.

LDA: Discriminant analysis can also be called discriminant function analysis. It distinguishes the data contained in the data set according to the characteristics it carries when assigning variable groups. Decriminant analysis is performed between a categorical dependent variable and independent variables that take numerical values. Discriminant analysis allows independent variables to be classified according to the same or different groups according to their influence on dependent variables.

*The purpose of discriminant analysis;

-To test whether it can be classified or not
-Classifying Variables
-Deconstructing the differences between groups
-To show the variance explained by the independent variables in the dependent variable
-In the classification according to the dependent variable, to examine the order of priority of the independent variables
-Eliminating variables that are of low importance (insignificant) when separating groups

ANOVA and MANOVA: ANOVA is used to Decipher whether there are differences between 3 or more groups based on a specific variable. MANOVA is a technique used to perform analysis of variance in experiments in which there are more than one dependent variable. The only difference from ANOVA is that there are more than one dependent variable.

ANOVA is similar to the LDA method. In two methods, it is the analysis of one or more categorical independent variables with a dependent variable. The ANOVA looks Decisively at whether the mean between the groups is equal or not.

Chi-Square: Used to Decipher the relationships between groups using the frequency distribution of categorical variables.

We also look at Information Gain.

NOTE: Filter methods do not prevent Multiple Linear Connections. Therefore, it is necessary to work separately for the ECD before installing the model.

*Wrapper Methods
![image](https://user-images.githubusercontent.com/97338597/186583120-12f5f37c-b47b-4ead-b2ca-68ebbfc4cc54.png)

They are stepwise methods. By adding and subtracting features to the model, the best model is tried to be found. It takes a long time to calculate.

-Forward Selection
-Backward Elimination
-Recursive Feature Elimination: Greedy Optimization Algorithm tries to find the features that will perform best).
-The Boruta algorithm performs well in Wrapper methods.

Wrapper yöntemlerinde Boruta algoritması iyi performans gösterir.

*Embedded Methods
![image](https://user-images.githubusercontent.com/97338597/186583281-1fc300a3-3a6e-4841-96d6-02ecae282c3e.png)

Embedded methods Use a combination of Filter and Wrap methods. Decoupling the filter and Wrap methods. The most popular embedded methods are LASSO, Elastic Net and RIDGE Regression. Reduces overfitting with punishing parameters.

In addition, the Regularized trees, Memetic algorithm, Random Multinomial Logit methods are also included in the embedded method.

*The Differences Between Filter and Wrapper Methods Decouple

-In filter methods, the relationship of independent variables with the dependent variable is examined. In the Wrapper method, it is checked whether the variables will work in the model.
-Filter methods are easier and faster than Wrapper methods. However, like wrapper methods, they are not included in the training phase of the model.
-Filter methods create subsets of properties using statistical methods. Wrapper methods, on the other hand, use Cross Validation.
-Filter methods may fail to select the best properties, but Wrapper methods always provide the best properties.
-There is a tendency to overfitting using Wrapper methods compared to filter methods.
