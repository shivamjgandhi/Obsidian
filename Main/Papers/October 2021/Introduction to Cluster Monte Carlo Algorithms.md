**Main Ideas**
- III: [[Swendsen-Wang Algorithm]]
	- A "bond" is formed between every pair of nearest neighbors that are aligned with probability $p_{ij} = 1 - exp(-2 \beta J)$, with $J$ as the coupling constant
	- All spins that are connected, directly or indirectly, via bonds belong to a single cluster. Thus, the assignment procedure divides the system into clusters of parallel spins
	- All spins in each cluster are flipped collectively with probability 1/2
	- All bonds are erased and the cluster move is complete. A new spin config has been created

