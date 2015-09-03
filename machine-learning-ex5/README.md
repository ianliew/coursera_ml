
# linearRegCostFunction.m

Straight forward implementation of the `J_theta` as provided in the exercise.

Linear regression here instead of logistic regression. So no `sigmoid`. Refer back to `computeCost.m` from ex1.

# learningCurve.m

Here, we are plotting learning curves based on the sample size.

Use `trainLinearReg` to train on X with sample size 1, 2, 3, etc ..., and `linearRegCostFunction` to spit out the cost/error for each iteration, making sure lambda = 0.

# polyFeatures.m

Built this using a for-loop. Wondering if this can be vectorized.

# validationCurve.m

Like `learningCurve.m`, instead of sample size, lamba is the variable here.

Use `trainLinearReg` to train the different lambdas, and `linearRegCostFunction` to spit out the cost. Again, lambda for `linearRegCostFunction` should be 0.
