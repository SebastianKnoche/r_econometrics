---
title: "GROUP ASSIGNMENTS"
subtitle: "Due to 2021-05-12"
author: "NAMAZI | SCHMALHOFER | KNOCHE"
date: "2021-05-05"
output:
  html_document:
    keep_md: yes
  pdf_document: default
---



***
## Chapter 3 - 5

In a study relating college grade point average to time spent in various activities, you distribute a survey to several students. The students are asked how many hours they spend each week in four activities: studying, sleeping, working, and leisure. Any activity is put into one of the four categories, so that for each student, the sum of hours in the four activities must be 168.

1. In the model $$GPA = \beta_{0} + \beta_{1} study + \beta_{2} sleep + \beta_{3} work + \beta_{4} leisure + u,$$ does it make sense to hold sleep, work, and leisure fixed, while changing study?

> No, it wouldn't make sense.

2. Explain why this model violates Assumption MLR.3.

> $$GPA = \beta_{0} + \beta_{1} study + \beta_{2} sleep + \beta_{3} work + \beta_{4} leisure + u = 168$$ This implies that $$\beta_{1} study + \beta_{2} sleep + \beta_{3} work + \beta_{4} leisure \hat{ = } 168.$$ Accordingly any summand is calculable through the equation.

3. How could you reformulate the model so that its parameters have a useful interpretation and it satisfies Assumption MLR.3?

> Leaving out any one coefficient (i.e. sleep) would suffice to satisfy MLR.3 .

***
## Chapter 3 - 7

Which of the following can cause OLS estimators to be biased?

1. Heteroskedasticity.

> Yes.

2. Omitting an important variable.

> Yes.

3. A sample correlation coefficient of 0.95 between two independent variables both included in the model.

> No, but it would not be desirable.

***
## Chapter 3 - C6

Use the data set in `wage2.dta` for this problem. As usual, be sure all of the following regressions contain an intercept.

1. Run a simple regression of `IQ` on `educ` to obtain the slope coefficient, say, $\tilde{ \delta_{1} }$.


```
## [1] "IQ = 53.6872 + 3.5338 educ + u"
```

```
## [1] "R^2 = 26.59 %"
```

```
## [1] "Sample size = 935"
```

```
## [1] "tilde-delta1 = 3.5338 educ"
```

2. Run the simple regression of log(`wage`) on `educ`, and obtain the slope coefficient, $\tilde{ \beta_{1} }$.


```
## [1] "log(wage) = 5.9731 + 0.0598 educ + u"
```

```
## [1] "R^2 = 9.74 %"
```

```
## [1] "Sample size = 935"
```

```
## [1] "tilde-beta1 = 0.0598 educ"
```

3. Run the regression of log(`wage`) on `educ` and `IQ`, and obtain the slope coefficients, $\hat{ \beta_{1} }$ and $\hat{ \beta_{2} }$ , respectively.


```
## [1] "log(wage) = 5.6583 + 0.0391 educ + 0.0059 IQ + u"
```

```
## [1] "R^2 = 12.97 %"
```

```
## [1] "Sample size = 935"
```

```
## [1] "hat-beta1 = 0.0391 educ"
```

```
## [1] "hat-beta2 = 0.0059 IQ"
```

4. Verify that $\tilde{ \beta_{1} } = \hat{ \beta_{1} } + \hat{ \beta_{2} } \tilde{ \delta_{1} }$.


```
## [1] "0.0598 = 0.0391 + 0.0059 * 3.5338"
```

```
## [1] "0.0598392035254231 = 0.0598392035254231"
```


***
## Chapter 3 - C7

Use `bwght2.dta` to answer this question.

1. Estimate the model $$log(bwght) = \beta_{0} + \beta_{1} cigs + \beta_{2} npvis + u,$$
and report the results in the usual form, including the sample size and R-squared. Are the signs of the slope coefficients what you expected? Explain.


```
## [1] "log(bwght) = 8.0555 + -0.0032 cigs + 0.0056 npvis + u"
```

```
## [1] "R^2 = 1.59 %"
```

```
## [1] "Sample size = 1832"
```
> Yes, a negative sign of the slope was expected due to the effects of cigarette smoking during pregnancies.

2. If `npvis` increases by one sample standard deviation, what is the estimated effect on birth weight?


```
## [1] "The estimated effect on bwght is 2.07 %, for an increase in npvis by 3.6808 ."
```

3. Now run the simple regression of log(`bwght`) on `cigs`, and compare the slope coefficient with the estimate obtained in part 1. Is the estimated effect of cigarette smoking much different than in part 1?


```
## [1] "log(bwght) = 8.121 + -0.0034 cigs + u"
```

```
## [1] "R^2 = 0.53 %"
```

```
## [1] "Sample size = 1832"
```

```
## [1] "The estimated effect of cigarette smoking is very similar, but slightly stronger than in part 1."
```

```
## [1] "The slope changes by: -0.3155 % - -0.3436 % = 0.0281 %."
```


4. Find the correlation between `cigs` and `npvis` and use it to explain the similarity of the simple and multiple regression estimates of $\beta_{1}$.


```
## [1] "The correlation coefficient is -0.0387 , the relationship between cigs and npvis is very vague and negative."
```

```
## [1] "Appearingly, not only the causality (explained through the regression) but also the correlation of cigs and npvis is very small and therefore the difference between the simple regression and the multiple regression is also very small (greater similarity)."
```


5. Add the variables `mage`, `meduc`, `fage`, and `feduc` to the regression from part (i). Is birth weight [more precisely log(`bwght`)] an easy variable to explain?


```
## [1] "log(bwght) = 7.9957 + -0.0025 cigs + 0.005 npvis + -8e-04 mage + -0.0013 meduc + 0.0022 fage + 0.0028 feduc + u"
```

```
## [1] "R^2 = 1.69 %"
```

```
## [1] "Sample size = 1832"
```

```
## [1] "Since R^2 is only 1.69 % and all coefficients are smaller than or equal to 0.5%, log(bwght) is a rather difficould variable to explain."
```
