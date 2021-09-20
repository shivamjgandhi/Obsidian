**Main Ideas**
- Monotonicity of [[Boolean function]]: a function is monotone if f(x) $\leq$ f(y) whenever x_i $\leq$ y_i
- [[Critical point]] - the center of where a transition occurs, $p_c$, where $E_p[f] = 1/2$. Fix some $\epsilon$ and we have that $E_{p_\epsilon}[f] = \epsilon$. 
- Lemma 8.5 (Margulis-Russo): the derivative of a function $p -> E_p[f]$, where the expectation is monotone, is equal to the expectation of the gradient's norm.
- The slope of the above function is the RHS of the [[Poincare inequality]]
- Cor 8.6 (Bollobas-Thomson): for all monotone Boolean functions, the width of the critical window is at most $C(\epsilon)=min(p_c, 1-p_c)$ where $C(\epsilon) = (\frac{1-\epsilon}{\epsilon})^{1/\epsilon} - 1 > 0$
- We say a monotone Boolean function exhibits a sharp transition if $p_{1-\epsilon} -p_{\epsilon} << min(p_c, 1-p_c)$

**Proof Techniques**
- Supremum at 1 and infimum at 0 if the [[Boolean function]] is monotone
- The variance of Boolean functions has special decompositions

**Intuititions Developed**
- Derivative of Boolean function based on supremum and infimum. 
- Can use indicator functions on Boolean functions to allow for $\geq$ and $\leq$
- The presence of a sharp transition is dependent on if fluctations are tiny as suggested by the Poincare inequality when in the critical window

**Questions**
- Poincare inequality