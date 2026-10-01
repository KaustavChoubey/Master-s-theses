# arw

# Activated Random Walks

This repository contains my Part III essay on **Activated Random Walks (ARW)**, written as part of my Master's studies in mathematics.

Activated Random Walks are an interacting particle system exhibiting a phase transition between **fixation** and sustained **activity**. They provide a mathematically tractable model related to the Abelian Sandpile and the broader phenomenon of **self-organised criticality**.

The essay develops the mathematical framework of ARW and works toward the result that, for every dimension $d\geq 1$ and every finite sleep rate $\lambda$,

$$
\mu_c(\lambda)<1,
$$

where $\mu_c(\lambda)$ denotes the critical particle density separating the fixating and active regimes.

## The Model

Particles move on the lattice $\mathbb{Z}^d$ and may be either **active** or **sleeping**.

Active particles perform random walks and attempt to fall asleep at rate $\lambda$ when alone. A sleeping particle becomes active again when another active particle reaches its site.

The competition between diffusion, sleeping and reactivation gives rise to a phase transition governed by the particle density $\mu$.

For each $\lambda$, there is a critical density $\mu_c(\lambda)$ separating two regimes:

$$
\mu < \mu_c(\lambda)
\quad\Longrightarrow\quad
\text{fixation},
$$

while

$$
\mu > \mu_c(\lambda)
\quad\Longrightarrow\quad
\text{continued activity}.
$$

## Main Topics

The essay develops several tools used in the study of Activated Random Walks, including:

- the **Diaconis–Fulton construction** and toppling formalism;
- monotonicity and abelianness properties;
- odometer functions and stabilisation;
- reduction from ARW on $\mathbb{Z}^d$ to finite discrete tori;
- coupling with a one-dimensional Markov chain;
- hitting probabilities for random walks on discrete tori;
- reversible Markov chains and bounds on stabilisation times;
- hierarchical dormitories, distinguished vertices and coloured loops;
- recursive toppling strategies and the **ping-pong argument**.

## A First Reduction: Stabilisation on Discrete Tori

An important step is to relate activity of the infinite system to the time required to stabilise ARW on the finite torus

$$
\mathbb{Z}_n^d=(\mathbb{Z}/n\mathbb{Z})^d.
$$

The analysis seeks regimes in which the stabilisation time $T_n$ is exponentially large with overwhelming probability:

$$
\mathbb{P}_{\mu}^{\lambda}
\left(
T_n < e^{c n^d}
\right)
<
e^{-c n^d}.
$$

To obtain such estimates, the toppling process can be coupled to a one-dimensional Markov chain. A greedy ordering of possible sleeping sites then provides geometric control over its drift.

This gives a relatively concrete route from the interacting particle system to questions about random walks, hitting probabilities and reversible Markov chains.

## Critical Density

The central result studied in the essay is

$$
\boxed{\mu_c(\lambda)<1}
$$

for every finite $\lambda>0$ and every $d\geq1$.

Particular attention is given to the historically difficult two-dimensional case. The essay studies quantitative upper bounds on $\mu_c(\lambda)$ in both the **low sleep-rate** and **high sleep-rate** regimes.

The proof introduces a hierarchical organisation of possible sleeping sites into **dormitory hierarchies**. Together with coloured loops, distinguished vertices and recursive toppling strategies, this provides control over the number of topplings required for stabilisation.

## Mathematical Themes

The project sits at the intersection of

**Probability · Interacting Particle Systems · Random Walks · Markov Chains · Percolation / Statistical Mechanics · Self-Organised Criticality**

## References and Attribution

This is an **expository Master's essay**, not a claim of original discovery of the main theorem.

The central result and quantitative bounds discussed in the essay are based primarily on the work of **Amine Asselah, Nicolas Forien and Alexandre Gaudillière**, together with earlier developments in the Activated Random Walk literature.

Full references and attribution are provided in the essay.

## Essay

The complete PDF is available in this repository:

**Activated Random Walks — Kaustav Choubey**
