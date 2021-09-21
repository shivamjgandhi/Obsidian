**Main Idea**

If we're trying to do multiclass classification, [[Linear Discriminant Analysis]] is when the covariance matrix is shared for all of the multivariate Gaussians that we're using to model our classes.

What happens is that we get decision functions called linear discriminant functions:

$\delta_k(x) = x^T \Sigma^{-1} \mu_k -1/2 \mu_k^T \Sigma^{-1} \mu_k +log(\pi_k)$ 

over which we may argmax and get the class. 

All of the decision boundaries end up being linear if we look at the log ratios. 