---
layout: home
title: Luca Mondada | DPhil Oxford Quantum Group
---


## Current research
Quantum compilation needs to scale up to
_i)_ handle large programs,
_ii)_ leverage everything from heterogenous HPC environment, and
_iii)_ generalise to non-unitary operations, real-time control flow, error correction etc.

We argue that interpreting quantum compilation as a graph transformation
system (GTS) is an elegant, flexible and scalable design for quantum compilers
that will enable these goals.
My recent contributions (to be pubished with my thesis) resolve the main
bottlenecks that GTS-based program optimisation faces, namely the slow rule
pattern matching in large rule systems and 
the difficulty of optimal rule application ordering, a.k.a. the phase ordering
problem, as it is known in classical compilation.

The first problem is solved by the introduction of a rule pre-compilation step,
during which all rules to be applied are aggregated into a _pattern matcher_,
a finite state automaton-like data structure that can be used to efficiently
to traverse a program graph and find all possible rule applications.
The paper [2] proves asymptotic bounds on the runtime of this approach for
the case of quantum circuits---with a runtime that is independent of the number
of rules in the system.

For optimal rule ordering, on the other hand, we propose a distributed search
algorithm that relies on the local Church-Rosser theorem to decompose the
search space into local problems that can be solved independently.
An MPI-based protocol is then used to merge local results into a provably optimal
global solution (within the explored search space), using a SAT solver.

Stay tuned for my thesis, coming soon! Oh, and don't hesitate to reach out in
the meantime, always happy to chat.

## Publications
 1. Koch M., Borgna A., Sivarajah S., et al. "HUGR: A Quantum-Classical Intermediate Representation."
  _Fifth International Workshop on Programming Languages for Quantum Computing, PLanQC 2025_. [[extended abstract](https://quantum-compilers.github.io/iwqc2024/papers/IWQC2024_paper_14.pdf)]
 2. Mondada, L. and Andrés-Martínez P. "Scalable Pattern Matching in Computation Graphs." 
 3. Mondada, L. "Quantum Circuits in Additive Hilbert Space.", preprint. [[2111.01211](https://arxiv.org/abs/2111.01211)]
  _15th International Workshop on Graph Computation Models, GCM 2024_. [[arxiv:2402.13065](https://arxiv.org/abs/2402.13065)]
 3. Corinzia, L., Penna, P., Mondada, L., Buhmann, J. M. (2019). "Exact Recovery for a Family of Community- Detection Generative Models."
   _IEEE International Symposium on Information Theory, ISIT 2019_, 415 – 419. [[arxiv:1901.06799](https://arxiv.org/abs/1901.06799)]
 4. Iten, R., Reardon-Smith, O., Mondada, L., Redmond, E., Kohli, R. S., & Colbeck, R. (2019).
   "Introduction to UniversalQCompiler." preprint [[arXiv:1904.01072](https://arxiv.org/abs/1904.01072)]
 5. Mondada, L., Karim, M.E., and Mondada, F. "Electroencephalography as implicit communication channel for proximal interaction between humans and robot swarms."
   _Swarm Intelligence_ 10.4 (2016): 247-265 [[pdf](https://infoscience.epfl.ch/record/221632/files/EEG-HSI.pdf)].

## Other past research and essays
 * Abstract Primitives for Quantum Computation. [[Term paper]{{ '/assets/docs/prim-review.pdf' | relative_url }}]
 * Simulating continuous-variable quantum computations on discrete devices.
   [[MFoCS dissertation]({{ '/assets/docs/dissertation.pdf' | relative_url }})]
 * An exploration of the meaning of Born's rule. [[miniproject]({{ '/assets/docs/qi_ht20.pdf' | relative_url }})]
