**Indicator Random Variable Method of Classification**
Using [[linear regression]] model on a indicator response matrix $Y \in R^{N \times K}$ where $N$ is the number of samples and $K$ is the number of classes. We have indicator random variables $Y_k = 1$ if $G=k$. 

Then to classify an observation:
1. compute the fitted output $\hat{f}(x)^T = (1, x^T)\hat{B}$, a $K$ vector
2. identify the largest component and classify accordingly:
$\begin{equation}\hat{G} = argmax_{k \in G} \hat{f_k}(x)
\end{equation}$

Rationale?
1. Can view this as an estimate of the conditional expectation for $Y_k$ where $E[Y_k |X=x] = P(G=k | X=x)$