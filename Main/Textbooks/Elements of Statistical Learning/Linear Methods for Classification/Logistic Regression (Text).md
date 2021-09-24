**Main Ideas**
- [[logistic regression]] model is used to model the posterior
- To fit the regression, we maximize the [[log likelihood]] of the [[multinomial distribution]]. This is done by setting the derivatives to 0 and getting score equations
- To solve the score equations we use the Newton-Raphson algorithm
- Convenient to write the score and Hessian in matrix notation. For the 2 class case, we create a matrix W that's NxN diagonal matrix of weights with the ith diagonal as p(x, beta)(1-p(x, beta)). Call p the vector of fitted probabilities. Then we have that we re-express the Newton step as a least squares [[linear regression]]. 

**Equations**

Equation for logistic regression for K classes
![[Pasted image 20210924103228.png]]

When comparing the probabilities for multiple classes
![[Pasted image 20210924103337.png]]

Newton-Raphson algorithm
![[Pasted image 20210924103543.png]]

Newton step for log reg
![[Pasted image 20210924103828.png]]

z is called the adjusted response

**Uses**
Good for an inference tool and for understanding the input variables