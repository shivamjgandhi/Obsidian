- [[MCMC]] often used to sample [[random variables]] for [[inference]]. Two shortcomings though
	- Although guaranteed to find a globally optimal solution given enough time, difficult to tell how close they are to a good solution given finite time
	- Choosing a good sampling technique is hard

**Inference as Optimization**
- Main idea is to cast inference as an optimization problem
- $p$ is intractable. Class of tractable distributions $Q$. Want some $q \in Q$ to approximate $p$
- Difference between sampling and variational techniques:
	- Variational approaches almost never find an optimal solution
	- We'll always know if they've converged
	- They scale better

**Variational Lower Bound**
- Fix a form for $p$. Assume $p$ is an [[undirected model]] of form 
![[Pasted image 20211007103237.png]]
where $\phi_k$ are [[factors]]
- We work with something called the [[ELBO]]:
![[Pasted image 20211007104140.png]]
- The ELBO has the property:
![[Pasted image 20211007104226.png]]
- Minimizing $J(q)$ amounts to maximizing a lower bound on the log likelihood $log p(D)$ of the observed data

**Further Questions**
- What does it mean for variational methods to scale better?
- What does it mean for a distribution to be directed or undirected?
- 