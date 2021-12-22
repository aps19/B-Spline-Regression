# B-Spline-Regression
To overcome the limitations of Linear Regression we can use an improved technique in which we can split the training data into multiple bins 
and fit each bin with a different model. This technique is known as the Regression spline.

## Knots and Bins
The points where division occurs are called Knots and the intervals or pieces of data are called bins.
The functions used to fit each bin are called Piecewise functions. These piecewise
functions can be of linear of polynomial types, here we have used a cubic polyomial.

## Piecewise Function
C0(X) = I(X < k0)<br />
C1(X) = I(k0 < k1)<br />
C2(X) = I(k1 < k2)<br />
.<br />
.<br />
.<br />
Cm(X) = I(km)<br />
where k0, k1, k2......km are the cut points and I(condition) is the function that return 1 when condition=True.<br />
Instead of fitting the same function over different bins of X. We fitted a cubic
Piecewise Polynomial over 5 bins. 

## Basis Function
Idea behind using low degree polynomial is to avoid high oscillations of the curve. Instead of treating the functions that are applied to the
bins as linear, it would be even more efficient to treat them as non-linear. To do this, a very general family of functions is applied to the variable. This family should
nor be too flexible to over-fit neither be too rigid to under-fit. These families of functions are called basic functions.

## Dataset
The Dataset used in this project is called Boston House Price Prediction(easily available on Kaggle). This dataset contains 506 Observations and 14 Variables.
1. CRIM (per capital crime rate by town)<br />
2. ZN (proportion of residential land zoned for lots over 25,000 sq.ft.)<br />
3. INDUS (proportion of non-retail business acres per town)<br />
4. CHAS (Charles River dummy variable (= 1 if tract bounds river; 0 otherwise))<br />
5. NOX (nitric oxides concentration (parts per 10 million)<br />
6. RM (average number of rooms per dwelling)<br />
7. AGE (proportion of owner-occupied units built prior to 1940)<br />
8. DIS (weighted distances to five Boston employment centers)<br />
9. RAD (index of accessibility to radial highways)<br />
10. TAX (full-value property-tax rate per 10,000 USD)<br />
11. PTRATIO (pupil-teacher ratio by town)<br />
12. B (1000(Bk — 0.63)2 where Bk is the proportion of blacks by town)<br />
13. LSTAT (percent lower status of the population)<br />
14. MEDV (Housing Prices)<br />
