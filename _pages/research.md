---
layout: archive
title: "Research Topics"
permalink: /research/
author_profile: true
---


I have been working on quantum computing, quantum information, and quantum many-body physics. Below let us explore  a few topics that I have been interested in.

**Quantum algorithms**

Quantum problems can be broadly classified into two categories: static problems and dynamics problems. Static problems correspond to finding a quantum system's lowest energy state or its eigenstate. Applications range from drug design to uncovering novel phases of matter, which, to most extent, can be transformed into an eigenstate problem. On the other hand, dynamics problems include finding quantum circuits to approximate the dynamics governed by a Hamiltonian, also known as Hamiltonian simulation, with applications including identifying dissipative phase transitions and studying information scrambling and transport.  

I have been working on improving algorithmic complexity in both of these general classes of quantum problems.

For static problems (i.e. finding eigenvalues and eigenvectors), we have developed several quantum algorithms. One example is a near-optimal eigenstate preparation method, termed quantum algorithmic cooling, which exhibits an exponential speedup in circuit complexity compared to conventional quantum algorithms like quantum phase estimation. Remarkably, algorithmic cooling operates deterministically without relying on assumptions about parametrised circuits and can guarantee simulation accuracy with near-optimal query complexity in precision, gap, etc. This matches the results by QSP and QETU while showing an advantage over quantum phase estimation and variational methods.

In more recent work, we provide a full-stack design of a quantum algorithm which considers the gate complexity, as opposed to previous algorithms based on querying either block encoding of the Hamiltonian and time evolution. We show that it maintains near-optimal system size and precision scaling.



**Quantum error mitigation and its transitions to quantum error correction**

I have been wondering how to overcome the fundamental limits set up by QEM. This motivates us to think about an intermediate form between QEM and QEC.

**Quantum computational chemistry**

The application of quantum computing to computational chemistry faces various experimental and theoretical challenges. Here, we address the critical challenges associated with solving molecular electronic structures using noisy quantum processors. We demonstrated a quantum simulation that in theory goes beyond the mean-field level. We achieved chemical accuracy for small molecules.

The protocol presents significant improvements in the circuit depth and running time, key metrics for chemistry simulation. Through systematic hardware enhancements and the integration of error mitigation techniques, we push forward the limit of quantum computational chemistry and successfully scale up the implementation of VQE with an optimised unitary coupled-cluster ansatz. We produce high-precision results of the ground-state energy for molecules with error suppression by around two orders of magnitude. 
 
 **Quantum many-body phenomena**

I have been interested in interesting many-body phenomena since my undergraduate study. I wonder if we could have a better understanding of emergent quantum phenomena in quantum materials.

I have worked on HTSC.
