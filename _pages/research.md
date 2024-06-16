---
layout: archive
title: "Research Topics"
permalink: /research/
author_profile: true
---


I have been working on quantum computing, quantum information, and quantum many-body physics. Below let us explore  a few topics that I have been interested in.

**Quantum algorithms**

Quantum problems can be broadly classified into two categories: static problems and dynamics problems. Static problems correspond to finding a quantum system's lowest energy state or its eigenstate. Applications range from drug design to uncovering novel phases of matter, which, to most extent, can be transformed into an eigenstate problem. On the other hand, dynamics problems include finding quantum circuits to approximate the dynamics governed by a Hamiltonian, also known as Hamiltonian simulation, with applications including identifying dissipative phase transitions and studying information scrambling and transport.  

I have been working on improving algorithmic complexity in both of these general classes of quantum problems. For static problems (i.e. finding eigenvalues and eigenvectors), we have developed several quantum algorithms. One example is a near-optimal eigenstate preparation method, termed quantum algorithmic cooling, in colloboration with Pei and Xiao. The algorithmic cooling operates deterministically without relying on assumptions about parametrised circuits and can guarantee simulation accuracy with near-optimal query complexity in precision, gap, etc. The query complexity (of real-time evolution) matches the results by QSP and QETU, while showing an advantage over quantum phase estimation and variational methods. 

In more recent work, we provide a full-stack design of a quantum algorithm which considers the gate complexity, as opposed to previous algorithms based on querying either block encoding of the Hamiltonian and time evolution. We show that it maintains near-optimal system size and precision scaling.



**Quantum error mitigation and its transitions to quantum error correction**

To effectively demonstrate the utility of quantum computing, we must confront challenges associated with the practical use of noisy quantum computers. Errors are an inherent aspect of quantum computing. Ensuring that quantum computing delivers accurate results in the presence of these errors is a critical consideration. Together with Suguru, Xiao, Vlatko and Simon, we initially proposed new QEM schemes to mitigate realistic noise described by Lindbladian appearing in both digital and analogue quantum devices. For noise from imperfections of the engineered Hamiltonian or additional noise operators, we show it can be effectively suppressed by a new QEM method, termed stochastic QEM. Our method only requires accurate single qubit controls, and is thus applicable to all digital quantum computers and various analogue simulators. This work inspires intensive follow-up research in the direction of QEM.

I have been wondering how to overcome the fundamental limits set up by QEM. This motivates us to think about an intermediate form between QEM and QEC. In recent work, we introduced an information-theoretic machinery, called a Quantum Filter, to purify or correct quantum channels. This addresses the sampling problem in QEM.


**Quantum computational chemistry**

The application of quantum computing to computational chemistry faces various experimental and theoretical challenges. Here, we address the critical challenges associated with solving molecular electronic structures using noisy quantum processors. We demonstrated a quantum simulation that in theory goes beyond the mean-field level. We achieved chemical accuracy for small molecules.

The protocol presents significant improvements in the circuit depth and running time, key metrics for chemistry simulation. Through systematic hardware enhancements and the integration of error mitigation techniques, we push forward the limit of quantum computational chemistry and successfully scale up the implementation of VQE with an optimised unitary coupled-cluster ansatz. We produce high-precision results of the ground-state energy for molecules with error suppression by around two orders of magnitude. 
 
 **Quantum many-body phenomena**

I have been interested in interesting many-body phenomena since my undergraduate study. I wonder if we could have a better understanding of emergent quantum phenomena in quantum materials, especially high-temperature superconductors. 

