
# lrCostFunction.m - Vectorizing the cost function, gradient (+ regularized)

Whilst I've implemented a vectorized cost function in **ex2**, and vectorizing the gradient wasn't all too hard since the formula has been provided... adding regularization to the cost function at j=0 (which is not to be regularized) is bit tricky.

The assignment suggested `temp = theta` and `temp(1) = 0`, I went the other way of returning `grad(1)` first, then `grad(2:end)`.

# oneVsAll.m

Challenge here was to understand what `fmincg` is returning and how it should be stored in `all_theta`.

# predictOneVsAll.m

I broke this problem down into getting the prediction for the first X

`sigmoid(X(1,:) * all_theta')`

then pick the MAX, then pick the index of MAX using the `max(A, [], 2)` hint.

# predict.m

Here is an additional step prior to applying MAX. Key is to understand the output that is required to feed into the next input.

`X[5000,400] -> X[5000,401] -> Theta1 -> X2[5000,25]`

`X2[5000,25] -> X2[5000,26] -> Theta2 -> X3[5000,10]`
