# Practical 6: Statistical Tests Using TeachingRatings Dataset

## Objective
To perform T-Test, ANOVA, Chi-Square Test, and Correlation on the TeachingRatings dataset.

## Q1. T-Test

**Question:** Using the teachers' rating dataset, does gender affect teaching evaluation rates?

**Results:**
- T-statistic: 3.2667
- P-value: 0.00117
- Significance level: 0.05
- Decision: Reject the Null Hypothesis

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant difference in teaching evaluation rates between male and female instructors.

## Q2. ANOVA Test

**Question:** Using the teachers' rating dataset, does beauty score for instructors differ by age?

**Results:**
- F-statistic: 10.9657
- P-value: 0.0000005749
- Significance level: 0.05
- Decision: Reject the Null Hypothesis

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant difference in beauty scores among the different age groups.

## Q3. Chi-Square Test

**Question:** Using the teachers' rating dataset, is there an association between tenure and gender?

**Results:**
- Chi-square statistic: 2.2068
- Degrees of freedom: 1
- P-value: 0.1374
- Significance level: 0.05
- Decision: Fail to Reject the Null Hypothesis

**Conclusion:** Since the p-value is greater than 0.05, we fail to reject the null hypothesis. There is insufficient evidence to conclude that tenure and gender are associated.

## Q4. Correlation Test

**Question:** Using the teachers' rating dataset, is teaching evaluation score correlated with beauty score?

**Results:**
- Correlation coefficient: 0.1890
- P-value: 0.00004247
- Significance level: 0.05
- Decision: Reject the Null Hypothesis

**Conclusion:** Since the p-value is less than 0.05, we reject the null hypothesis. There is a statistically significant positive correlation between teaching evaluation score and beauty score.

## Final Conclusion

In this practical, we performed four statistical tests on the TeachingRatings dataset. The T-Test showed a significant difference in evaluation rates by gender. ANOVA showed differences in beauty scores across age groups. The Chi-Square test found insufficient evidence of an association between tenure and gender. The correlation test showed a significant positive relationship between teaching evaluation scores and beauty scores.