# Bellman Expectation Equation — Vector Form Cheat Sheet

A compact 2-page reference card expressing the Bellman Expectation 
Equation as four vector dot products, with full variable definitions, 
a TikZ MDP diagram, and a complete glossary. Source included in XeLaTeX.

## What's novel

The Bellman Expectation Equation is the foundation of reinforcement 
learning, but standard presentations are either hard to read or hard 
to compute with:

- **Scalar/summation form** (Sutton & Barto style): precise but the 
  structure is buried in sigma notation
- **Matrix/operator form** (theoretical papers): elegant but abstract

This cheat sheet takes a middle path: four explicit vector dot products 
that expose the full computational skeleton of the equation in a form 
immediately readable to anyone with basic linear algebra.

The four steps are:

1. **g = γ⃗ · r⃗** — discounted return as a dot product
2. **o⃗ = r⃗ + γv⃗'** — outcome vector (one-step Bellman backup)
3. **q = p⃗ · o⃗** — state-action value as expected outcome
4. **v = π⃗ · q⃗** — state value as expected Q-value under policy

## Contents

- `Bellman_Expectation_Equation.pdf` — the cheat sheet (2 pages)
- `Bellman_Expectation_Equation.tex` — XeLaTeX source

## Who this is for

Students and practitioners who want to see the Bellman equation 
as a concrete linear algebra computation rather than an abstract 
expectation over probability distributions.

## Keywords
reinforcement learning, Bellman equation, Bellman expectation equation,
value function, Q-function, state-action value, policy, MDP, 
Markov decision process, cheat sheet, reference card, linear algebra, 
dot product, state value, action value, RL, dynamic programming, 
temporal difference, reward, discount factor, transition probability
-- Khosro Pourkavoos
