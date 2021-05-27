---
title: "GROUP ASSIGNMENTS"
subtitle: "Due to 2021-06-02"
author: "NAMAZI | SCHMALHOFER | KNOCHE"
date: "2021-04-30"
output:
  html_document:
    keep_md: yes
  pdf_document: default
---





# Chapter 5

## C1

Use the wage1 data for this exercise



### 1.    Estimate the equation

$wage = \beta_{0} + \beta_{1} educ + \beta_{2} exper + \beta_{3} tenure + u$



> $\begin{align*}
wage & = -2.8727 + (0.599) educ + (0.0223) exper + (0.1693) tenure + u \\  
R^{2} & = 30.6422\% ;    Sample size = 526 \\
\end{align*}$  

Plot a histogram of the residuals.

<div class="figure" style="text-align: center">
<img src="r_20210526_namazi_schmalhofer_knoche_files/figure-html/plot 1 wage model-1.png" alt="Plot 1: The frequency of the respective values for the residuals of the wage model"  />
<p class="caption">Plot 1: The frequency of the respective values for the residuals of the wage model</p>
</div>

### 2.    Repeat part 1 including plotting, but with log(wage) as the dependent variable.



> $\begin{align*}
lwage & = 0.2844 + (0.092) educ + (0.0041) exper + (0.0221) tenure + u \\  
R^{2} & = 31.6013\% ;    Sample size = 526 \\
\end{align*}$  

<div class="figure" style="text-align: center">
<img src="r_20210526_namazi_schmalhofer_knoche_files/figure-html/plot 2 log(wage) model-1.png" alt="Plot 2: The frequency of the respective (relative) values for the residuals of the log(wage) model"  />
<p class="caption">Plot 2: The frequency of the respective (relative) values for the residuals of the log(wage) model</p>
</div>

### 3.    Would you say that Assumption MLR.6 is closer to being satisfied for the level-level model or the log-level model?

> ?

## C2

Use the GPA2 dataset.



### 1.    Using all 4137 observations, estimate the equation

$colgpa = \beta_{0} + \beta_{1} hsperc + \beta_{2} sat + u$

and report the results in the usual form.



> $\begin{align*}
colgpa & = 1.3918 + (-0.0135) hsperc + (0.0015) sat + u \\  
R^{2} & = 27.3441\% ;    Sample size = 4137 \\
\end{align*}$  

### 2.    Reestimate the equation in part 1, using the first 2700 observations.



> $\begin{align*}
colgpa & = 1.4065 + (-0.0131) hsperc + (0.0015) sat + u \\  
R^{2} & = 27.1795\% ;    Sample size = 2700 \\
\end{align*}$  
