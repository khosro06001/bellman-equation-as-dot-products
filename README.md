# The Pourkavoos-Bellman Equation: Bellman Equations as Dot Products

I reformulated the Bellman Expectation Equation using three vector dot products 
instead of the usual nested summation notation. In two forms:

- Gibbs Notation (traditional vector notation)
- Einstein Notation

**Gibbs notation — four steps:**

1. **g = γ⃗ · r⃗** — discounted return as a dot product
2. **o⃗ = r⃗ + γv⃗'** — outcome vector (one-step Bellman backup)
3. **q = p⃗ · o⃗** — state-action value as expected outcome
4. **v = π⃗ · q⃗** — state value as expected Q-value under policy

**Einstein notation — the full equation in one line:**

v = π_i p_ij (r_ij + γ v'_j)

where i indexes actions and j indexes next states.

## What's novel

The Bellman Expectation Equation is the foundation of reinforcement learning, 
but standard presentations are either hard to read or hard to compute with:

- **Scalar/summation form** (Sutton & Barto style): precise but the structure 
  is buried in sigma notation
- **Matrix/operator form** (theoretical papers): elegant but abstract

This document takes a middle path: three explicit vector dot products that 
expose the full computational skeleton of the equation in a form immediately 
readable to anyone with basic linear algebra.

## Computational advantage

The dot product form maps directly to optimized library functions — numpy.dot(), 
torch.mv(), and hardware-accelerated routines — enabling efficient 
computation on both CPU and GPU. The nested summation form requires explicit 
loops or manual indexing; the dot product form hands the computation directly 
to vectorized library functions.

## Document

[Pourkavoos_Bellman_Expectation_Equation.pdf](Pourkavoos_Bellman_Expectation_Equation.pdf)

## Citation

Pourkavoos, K. (2026). The Pourkavoos-Bellman Equation: Bellman Equations as 
Dot Products (Version v79). Zenodo. https://doi.org/10.5281/zenodo.21462016

## Who this is for

Students and practitioners who want to see the Bellman equation as a concrete 
linear algebra computation rather than an abstract expectation over probability 
distributions.

## Keywords
reinforcement learning, Bellman equation, Bellman expectation equation,
value function, Q-function, state-action value function, state value function, 
policy, MDP, Markov decision process, linear algebra, dot product, Einstein 
notation, dynamic programming, reward, discount factor, transition probability

---

-- Khosro Pourkavoos

## Acknowledgements

I want to thank my great RL teacher, Professor Ausif Mahmood, for encouraging 
students to attempt to fully understand the derivation of the Equations. 
This was the motivation for this expedition, resulting in the above succinct 
formulation.
