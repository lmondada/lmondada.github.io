---
layout: home
title: Luca Mondada | DPhil Oxford Quantum Group
---


## Current research
I am trying to improve on our current approaches to quantum circuit simplification.
The circuit representation we use both for circuit design and optimisation poses indeed a few challenges.
It can be hard -- or unnatural -- to squeeze a quantum primitive into a circuit:
think of how a controlled unitary is decomposed into something unrecognisable in a typical
universal gate set.
On the user-facing design side, this might be patched by introducing new ad-hoc primitives as they are needed.
On the optimisation side, however, this causes problems: it is very hard to resynthesise higher-level
primitives from simpler ones, or to make use of ad-hoc primitives in a general way.

This means that we face difficulties in devising and using optimisation strategies that could leverage
this higher-level structure. Beyond circuit optimisation performance, this will increasingly become an important
issue if we wish to compile to architectures that might support more exotic gate sets than are currently typically
available, such as multi-qubit operations on ion traps devices.

I am currently formulating a new presentation of quantum computation that aims to address some of these issues.
Paper to come out on this very soon...

## Publications
 - Corinzia, L., Penna, P., Mondada, L., Buhmann, J. M. (2019). "Exact Recovery for a Family of Community- Detection Generative Models."
   _IEEE International Symposium on Information Theory, ISIT 2019_, 415 – 419. [[arxiv:1901.06799](https://arxiv.org/abs/1901.06799)]
 - Iten, R., Reardon-Smith, O., Mondada, L., Redmond, E., Kohli, R. S., & Colbeck, R. (2019).
   "Introduction to UniversalQCompiler." preprint [[arXiv:1904.01072](https://arxiv.org/abs/1904.01072)]
 - Mondada, L., Karim, M.E., and Mondada, F. "Electroencephalography as implicit communication channel for proximal interaction between humans and robot swarms."
   _Swarm Intelligence_ 10.4 (2016): 247-265 [[pdf](https://infoscience.epfl.ch/record/221632/files/EEG-HSI.pdf)].

## Other past research and essays
 * Simulating continuous-variable quantum computations on discrete devices.
   [[MFoCS dissertation]({{ '/assets/docs/dissertation.pdf' | relative_url }})]
 * An exploration of the meaning of Born's rule. [[miniproject]({{ '/assets/docs/qi_ht20.pdf' | relative_url }})]
