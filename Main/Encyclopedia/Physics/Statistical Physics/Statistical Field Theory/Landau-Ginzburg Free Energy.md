(Based off of David Tong's notes on statistical field theory)

**The Constraints on the Free Energy**
1. Locality ([[Markov property]]) 
$F[m(x)] = \int d^dx f[m(x)]$
where $f[m(x)]$ is a local function
2. Translational and rotational invariance
3. $Z_2$ symmetry
4. Analyticity

**Why would a linear term violate rotational symmetry?**
https://physics.stackexchange.com/questions/673914/why-does-a-linear-term-in-the-gradient-violate-rotational-symmetry 

Misc notes
- Hard to get coefficients for the free energy from first principles. We can get them via [[Landau theory]]
- The coefficient $\alpha_2$ flips signs at the [[second order phase transition]]

**Saddle Points and Domain Wells**
- We can use the [[Saddle point method]] to try to solve the functional integral. We assume the path integral is dominated by configs that minimize the free energy
- To find the min, we use [[variational methods]] and create a [[functional derivative]] that goes into the [[Euler-Lagrange equation]]
- The simplest solutions have $m$ constant and end up giving the result from Landau theory
- So the [[mean field approximation]] is just the saddle point approx in Landau Ginzburg theory

**Domain walls**
- In one dimension, the Euler Lagrange equation turns into a second order differential equation. If we insist that the field interpolates between the two ground states as x goes to infinity, then we get the solution [[tanh]]
$\begin{equation}m = m_0 \text{tanh}(\frac{x-X}{W})\end{equation}$
where X is the position of the domain wall and $W=\sqrt{-2 \gamma/\alpha_2}$.

**The Lower Critical Dimension**
- For a large enough system, $L/W$ will overwhelm any exponential suppression. The entropy of a config will outweigh the energetic cost.
- In terms of having $n$ walls, we get something exponential.
- The probability of having flipped signs by the end is related to the sinh function and the probability of not having flipped is related to the cosh function

**General principle**
- Whenever we've a L-G theory characterized by a symmetry, then the [[ordered phase]] will have a number of degenerate disconnected ground states which spontaneously break symmetry. In all such cases, the lower critical dimension is $d_l = 1$ and the underlying reason is the same, [[fluctuations]] of domain walls take us from one ground state to another and destroy ordered phase. 