**Formal Definition**
![[Pasted image 20211013163522.png]]

https://ermongroup.github.io/cs228-notes/representation/undirected/

Advantages of MRF vs [[Bayes nets]]
- Can be applied to a wider range of problems where there's no direction or variable dependence

Disadvantages
- Compute the [[partition function]] is usually [[NP-hard]]
- May be difficult to interpret
- Much easier to generate data in a Bayes net

- Independence between two sets of variables depends on a cut set. We then get a Markov blanket for a variable which just ends up being its neighbors

**Further questions**
- I want some intuition regarding what can be represented as a Bayes net vs. a MRF
- An HMM is similar to a chain CRF except that it has arrows between the hidden states and the outputs
