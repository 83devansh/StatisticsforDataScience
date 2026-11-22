# Practical 7: Regression Analysis Using TeachingRatings Dataset

## Objective
To perform regression analysis using T-test, ANOVA, and correlation on the TeachingRatings dataset.

## Q1. Regression with T-Test (Gender vs Evaluation)

**Question:** To determine if gender affects teaching evaluation rates.

**Results:**
- Number of observations: 463
- R-squared: 0.022
- F-statistic: 10.56
- Probability (F-statistic): 0.00124
- Female coefficient: -0.1680
- T-statistic: -3.250
- P-value: 0.001

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant difference in teaching evaluation rates between male and female instructors. The negative coefficient indicates that female instructors have lower average evaluation scores than male instructors in this dataset.

## Q2. Regression with ANOVA (Beauty vs Age Group)

**Question:** To check if beauty scores for instructors differ by age group.

Age groups:
- Young: 0–40
- Middle: 41–56
- Old: 57–100

**Results:**
- F-statistic: 17.5976
- P-value: 4.32255e-08

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant difference in beauty scores among the different age groups.

## Q3. Regression (Evaluation vs Beauty)

**Question:** To check the relationship between teaching evaluation scores and beauty scores.

**Results:**
- Number of observations: 463
- R-squared: 0.036
- F-statistic: 17.08
- Probability (F-statistic): 4.25e-05
- Beauty coefficient: 0.1330
- T-statistic: 4.133
- P-value: 0.000

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant positive relationship between beauty scores and teaching evaluation scores. The positive coefficient indicates that evaluation scores tend to increase as beauty scores increase.

## Final Conclusion

In this practical, we performed regression analysis using the TeachingRatings dataset. We studied the effect of gender on teaching evaluation scores, compared beauty scores across age groups, and examined the relationship between beauty and teaching evaluation scores. The results showed statistically significant relationships in all three analyses.