---
title       : Standard Normal Density App
subtitle    : Developing Data Products course project
author      : Naveen Mathew Nathan S.
job         : Student
framework   : io2012
highlighter : highlight.js
hitheme     : tomorrow
widgets     : [mathjax]
mode        : selfcontained
knit        : slidify::knit2slides
---

## Introduction to the shiny app

1. The app is built using shiny and hosted on shinyapps.io.
2. The app calculates probability of a score according to standard normal density.

--- .class #id 

## Math behind

1. A standard normal distributed variable is of form $X\sim N(0,1)$
2. The PDF is $f(x)=\frac{1}{\sqrt{2\pi}}e^{-\frac{1}{2}x^2}$
3. A upper tail probability for a score x is calculated using $P(X>x)$ 
4. A lower tail probability for a score x is calculated using $1-P(X>x)$ 

--- .class #id 

## R code

1. The probability is calculated using R function pnorm()

```r
x = 0.5
lower = T
pnorm(x, mean = 0, sd = 1, lower.tail = lower)
```

```
## [1] 0.6914625
```
2. The value for x and wether user wants a lower probability or a upper probability are based on user input.

--- .class #id 

## Thank you!
