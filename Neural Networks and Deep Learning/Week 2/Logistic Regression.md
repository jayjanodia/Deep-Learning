Given an input feature vector X, assume an image, we must predict y_hat, which is the estimate of y (P(y=1|x))

Given an input X (X dimensional vector) and parameters w (X dimensional vector) and b(which is just a real number), how would we generate the output y_hat. 

If we use the linear regression function y = w.T\*x + b, then we may get the outputs as -ve, but we know that in classification we can't have values less than 0 (for binary classification values range from 0 to 1). So, we are actully going to use the sigmoid of (w.T\*x + b) to get a better outcome. The formula for this is sigmoid(z) = 1/(1+e^-z). If z is large, sigmoid(z) will be close to 1, since e^z will be close to 0. If z is very small or a very large negative number, e^z would be close to a very large number and the outcome would be close to 0. 

## Cost Function

