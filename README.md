# Bellman Expectation Equation — Vector Form!

I reformulated the Bellman Expectation Equation using vector dot products instead of the usual summation sigma summation notation.

** g = γ⃗ · r⃗ **

** o⃗ = r⃗ + γv⃗' **

** q = p⃗ · o⃗  **

** v = π⃗ · q⃗ **


See: PDF

## What's novel

The Bellman Expectation Equation is the foundation of reinforcement 
learning, but standard presentations are either hard to read or hard 
to compute with:

- **Scalar/summation form** (Sutton & Barto style): precise but the 
  structure is buried in sigma notation
  
- **Matrix/operator form** (theoretical papers): elegant but abstract

This cheat sheet takes a middle path: 3 explicit vector dot products and 
a vector summation equation that expose the full computational skeleton 
of the equation in a form immediately readable to anyone with basic linear algebra.

The four steps are:

1. **g = γ⃗ · r⃗** — discounted return as a dot product
2. **o⃗ = r⃗ + γv⃗'** — outcome vector (one-step Bellman backup)
3. **q = p⃗ · o⃗** — state-action value as expected outcome
4. **v = π⃗ · q⃗** — state value as expected Q-value under policy

## Contents

- `Bellman_Expectation_Equation.pdf` — the cheat sheet (2 pages)

## Who this is for

Students and practitioners who want to see the Bellman equation 
as a concrete linear algebra computation rather than an abstract 
expectation over probability distributions.

Professors, who empathsize with students struggling to learn these concepts.

The Curious!

## Keywords
reinforcement learning, Bellman equation, Bellman expectation equation,
value function, Q-function, state-action value function, state value function, policy, MDP, 
Markov decision process, linear algebra, dot product, state value, action value, RL, dynamic programming, 
temporal difference, reward, discount factor, transition probability

-- Khosro Pourkavoos

:)
