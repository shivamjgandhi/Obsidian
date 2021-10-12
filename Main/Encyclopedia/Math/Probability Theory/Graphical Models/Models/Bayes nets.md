- Show causality and are directed whereas MRFs [[undirected model]] are undir.

**Probabilistic modeling with Bayes nets**
- Via the chain rule, 
![[Pasted image 20211012164859.png]]
a compact Bayes net is a dist. where each factor on the RHS depends only on a small number of ancestor variables $x_{A_i}$. 
- If each variable takes on $d$ values and has at most $k$ ancestors, then the entire table has at most $O(d^{k+1})$ entries so the whole P-dist is specified with $O(nd^{k+1})$ whereas the naive model has $O(d^n)$ params

**Graphical representation**
- DAG shows how [[random variables]] depend on each other
- Also can be thought of as a story to how data was generated
- The formal definition: 
![[Pasted image 20211012165133.png]]

**Dependencies of a Bayes Net**
- The 3 types of dependency structures:
![[Pasted image 20211012165253.png]]
- For the v-structure, suppose C is a boolean variable indicating whether the lawn is wet. A and B are two explanations for it being wet. A: it rained, B: sprinklers turn on. If we know C = 1, and B = 0, we know A = 1. Therefore A, B not ind given C
- Active path: 
![[Pasted image 20211012165430.png]]
- The idea behind an active path is a path where information can flow which destroys independence between the sets. Thus, d-separation is when there are no paths for information flow. Consecutive triples since that describes each "chain" in the path
- I-map: 
![[Pasted image 20211012165631.png]]
- Fact: if $p$ factorizes over $G$, then $I(G) \subset I(p)$ and we say that $G$ is an I-map for $p$. 
- If $G$ and $G'$ have the same skeleton (removal of directedness) and the same v-structures, then $I(G) = I(G')$.