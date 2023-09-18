# Chi-Square Test Analysis

This README provides an overview of the Chi-Square test analysis conducted on categorical features. The Chi-Square Test of Independence determines whether there is an association between categorical variables (i.e., whether the variables are independent or related). It is a nonparametric test.
The analysis aimed to determine whether there are significant differences between various pairs of categorical features.


## Hypotheses

In this analysis, tested the following hypotheses:

- **Null Hypothesis (H0)**: There is no significant difference between the levels of categorical_feature_1 and categorical_feature_2 (and similarly for other pairs).

- **Alternative Hypothesis (H1)**: There is a significant difference between the levels of categorical_feature_1 and categorical_feature_2 (and similarly for other pairs).

## Chi-Square Test Procedure

To test these hypotheses, I followed these steps:

1. Organized the data in a cross-tabulation (contingency) format, where each row represented a level (group) of one variable, and each column represented a level (group) of another variable.

2. Compared the calculated chi-square test statistics with critical values from a chi-square distribution table. The degrees of freedom were determined by (number of rows - 1) times (number of columns - 1).

3. The analysis was conducted at specific significance levels (0.01, 0.05, 0.001).

## Results

The results of the Chi-Square test indicated that all of the calculated chi-square test statistics exceeded the critical values for each significance level (0.01, 0.05, 0.001). Therefore, we rejected all null hypotheses, suggesting a significant difference between all pairs of categorical features. In other words, there is no relationship between any of the categorical features tested, including:

- `categorical_feature_1` & `categorical_feature_2`
- `categorical_feature_1` & `categorical_feature_3`
- `categorical_feature_1` & `categorical_feature_4`
- `categorical_feature_2` & `categorical_feature_3`
- `categorical_feature_2` & `categorical_feature_4`
- `categorical_feature_3` & `categorical_feature_4`

## Conclusion

This analysis provides valuable insights into the relationships between categorical features, helping us understand their independence or lack thereof.