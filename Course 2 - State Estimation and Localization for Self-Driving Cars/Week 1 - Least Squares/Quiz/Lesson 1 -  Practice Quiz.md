# Lesson 1 - Practice Quiz
---
**Question 1.**
In order to apply the method of least squares, it is necessary to know the measurement noise variances.

- [ ] True
- [x] False
```
Correct
Correct! Least squares can be applied to minimize a squared error criterion,
without necessarily knowing the noise characteristics of the measurements.
```

**Question 2.**
For the method of least squares, select any/all that apply.

- [ ] The squared error criterion and least squares method can be applied directly to nonlinear measurement models.

- [x] Given a linear observation model, the parameters that minimize the squared error criterion can be found by solving the normal equations.
```
Correct
Correct! However, there is an additional criterion required for the solution to be valid. For more details, review the "Squared Error Criterion and the Method of Least Squares" lecture in this module.
```

- [x] The method was pioneered by Carl Friedrich Gauss.
```
Correct
Correct! The least-squares method is usually credited to Carl Friedrich Gauss (1795).
```

**Question 3.**
Lesson 1 referred to the Jacobian matrix, \mathbf{H}H, which relates the parameters of the linear model to the measurements. Assume that, for a particular problem, our model has three parameters and we obtain ten measurements - what size should the Jacobian matrix be?

- [x] The matrix **H** should be 10 times 3 10×3 in size.

- [ ] The matrix **H** should be 3 times 10 10×10 in size.
```
Correct
Right! There is one row in the matrix for each measurement and one column for each parameter.
```
**Question 4.**
According to the weighted squared error criterion, the error term corresponding to a measurement with a noise variance of 10 units will be weighted more highly than that of a measurement with a noise variance of 1 unit.

- [ ] True

- [x] False
```
Correct
Correct! A larger noise covariance means a lower weight (i.e., a less trustworthy measurement).
```
**Question 5.**
In which of these cases would the method of weighted least squares produce valid solutions. Select any/all that apply.


- [ ] Five measurements, six unknown parameters.

- [x] Five measurements, five unknown parameters, and two different noise variances.
```
Correct
Correct! We have an equal number of measurements and unknowns, which means the
five parameters can be estimated correctly. The non-zero noise variances affect
the estimator accuracy, but not the validity of the solution.
```

- [ ] Ten measurements, two unknown parameters, and two different noise variances, one of which is exactly zero.

- [x] Ten measurements, two unknown parameters.
```
Correct
Correct! We have more measurements than unknowns, which means the two parameters
 can be estimated reliably.
```

**Question 6.**
You are measuring the voltage drop VV across an electrical component using two different multimeters; one of the meters is known to be more reliable than the other. Which method would you use to estimate the best voltage value from noisy measurements?


- [x] Weighted Least Squares

- [ ] Least Squares
```
Correct
Correct! WLS can handle the possibility of the measurements having different noise levels (variances).
```
