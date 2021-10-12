**Main Points**
- Broke down the expression variance into a spatial and non-spatial component
- The SpatialDE model was a multivariate normal model of form
$P(y|\mu, \sigma_{s}^2, \delta, \Sigma) = N(y | \mu, \sigma_s^2 \cdot (\Sigma + \delta \cdot I))$
where $\Sigma$ is the squared exponential covariance function
- $\delta \cdot I$ accounts for independent non-spatial variation in gene expression
- Model parameters fit via maximizing the marginal [[log likelihood]] given $\delta$
- For statistical significance, they compared the model likelihood of the fitted SpatialDE model with the likelihood of a model that corresponds to the null hypothesis of no spatial covariance:
$P(y |\mu, \sigma^2)=N(\mu, \sigma^2 \cdot I)$
- Estimated P-vals based on the [[chi-squared]] distribution with one degree of freedom
- Model selection done by comparing the [[Bayesian Information Criterion]]
- To group spatially variable genes with similar spatial expression patterns, SpatialDE implements a clustering model based on the same spatial [[Gaussian Process]] based prior
- Approximate the posterior distribution for $\mu, Z$ from [[variational inference]]
- $\sigma_e^2$ estimated by maximizing the [[ELBO]]
- After inference, posterior expectations for $\mu, Z$ of params can be used to visualize any histological pattern through plotting of the $\mu_k$ over the x coordinates

**Possible Things to Investigate**
- Comparison to HMRF method

**Questions**

**Extra Notes**