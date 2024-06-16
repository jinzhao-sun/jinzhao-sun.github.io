---
layout: archive
title: "Research Topics"
permalink: /research/
author_profile: true
---


I have been working on quantum computing, quantum information, and quantum many-body physics. Below let us explore  a few topics that I have been interested in.

Quantum computing
=====

Quantum problems can be broadly classified into two categories: static problems and dynamics problems. Static problems correspond to finding a quantum system's lowest energy state or its eigenstate. Applications range from drug design to uncovering novel phases of matter, which, to most extent, can be transformed into an eigenstate problem. On the other hand, dynamics problems include finding quantum circuits to approximate the dynamics governed by a Hamiltonian, also known as Hamiltonian simulation, with applications including identifying dissipative phase transitions and studying information scrambling and transport.  

I have been working on improving algorithmic complexity in both of these general classes of quantum problems. For static problems (i.e. finding eigenvalues and eigenvectors), we have developed several quantum algorithms. One example is a near-optimal eigenstate preparation method, termed quantum algorithmic cooling, in collaboration with Pei and Xiao. The algorithmic cooling operates deterministically without relying on assumptions about parametrised circuits and can guarantee simulation accuracy with near-optimal query complexity in precision, gap, etc. The query complexity (of real-time evolution) matches the results by QSP and QETU, while showing an advantage over quantum phase estimation and variational methods. More details could be found [here](https://arxiv.org/abs/2109.15304).

In more recent work, we provide a full-stack design of a quantum algorithm which considers the gate complexity, as opposed to previous algorithms based on querying either block encoding of the Hamiltonian and time evolution. We show that it maintains near-optimal system size and precision scaling. Details could be found [here](https://arxiv.org/abs/2406.04307).

**Dynamics problems**, i.e., simulating the dynamics of quantum systems, is a fundamental task in quantum physics and is believed to be a major application of quantum computers. Below, I introduce a few related works.

Perturbative approach to quantum dynamics simulation. Perturbation theory brings about great success in quantitative predictions of quantum mechanics; however, challenges remain in solving the major component and computing the power series. We addressed this challenge by developing a conceptually novel approach, perturbative quantum simulation (PQS), which exploits the complementary strength of quantum computing and perturbation theory. We demonstrated that PQS is applicable to simulate classically challenging systems, such as large systems with weak inter-subsystem interactions or intermediate systems with general interactions. Remarkably, PQS shows significant advantages over conventional quantum simulation algorithms concerning the quantum resource requirements and noise robustness. I have explored applications in interacting bosons, fermions, and quantum spins in different topological structures and studied different quantum phenomena on systems of up to 48 qubits, such as information propagation, charge-spin separation, magnetism, etc. Details could be found [here](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.129.120505).

Adaptive product formulae. We introduced an adaptive product formula which can produce a compact quantum circuit for Hamiltonian simulation. We introduced a measurable quantifier to describe the dynamics simulation error. The simulation error is rigorously analysed. The adaptive product formula is proven to guarantee simulation accuracy, showing an advantage over conventional product formula methods or variational quantum algorithms. Our method can be used as a subroutine of many quantum algorithms, and we demonstrated the applications for solving eigenvalue problems in quantum chemistry. Our work largely reduces quantum resources for Hamiltonian simulation and thus enables practical implementation with near-term or early fault-tolerant quantum devices. Details could be found [here](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.130.040601).

**Quantum computing and spectroscopy**

Estimating spectral features of quantum many-body systems has attracted great attention in material science
and quantum chemistry. To achieve this task, various experimental and theoretical techniques have been developed, including spectroscopy techniques, and quantum simulation either by engineering controlled quantum
devices or executing quantum algorithms. However, probing a quantum system's behaviour is challenging and demands substantial resources for both approaches. For instance, real probe by neutron spectroscopy requires access to large-scale facilities with high-intensity neutron beams, while quantum computing of eigenenergies, such as phase estimation, typically requires a long coherence time in engineering controlled quantum devices. In a recent project, we established a framework for probing the excitation spectrum of quantum many-body systems with quantum simulators. More details could be found [here](https://arxiv.org/abs/2305.07649).

I have been thinking of the crossover between static problems and dynamics problems, well-established spectroscopy techniques and quantum computing. Some philosophical discussions on quantum machinery and spectroscopy can be found in my [thesis](https://ora.ox.ac.uk/objects/uuid:de5499cb-9c49-4be3-acc1-5be4cb81099d).


**Quantum error mitigation and its transitions to quantum error correction**

To effectively demonstrate the utility of quantum computing, we must confront challenges associated with the practical use of noisy quantum computers. Errors are an inherent aspect of quantum computing. Ensuring that quantum computing delivers accurate results in the presence of these errors is a critical consideration. Together with Suguru, Xiao, Vlatko and Simon, we initially proposed new QEM schemes to mitigate realistic noise described by Lindbladian appearing in both digital and analogue quantum devices. For noise from imperfections of the engineered Hamiltonian or additional noise operators, we showed it can be effectively suppressed by a new QEM method, termed stochastic QEM. Our method only requires accurate single qubit controls, and is thus applicable to all digital quantum computers and various analogue simulators. Details could be found [here](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.15.034026).

I have been wondering how to overcome the fundamental limits set up by QEM. This motivates us to think about an intermediate form between QEM and QEC. In recent work, we introduced an information-theoretic machinery, a commutation-derived quantum filter, to purify or correct quantum channels. This addresses the sampling problem in QEM.


**Quantum computational chemistry**

The application of quantum computing to computational chemistry faces various experimental and theoretical challenges. In a recent project with USTC and Peking, we addressed the critical challenges associated with solving molecular electronic structures using noisy quantum processors. We demonstrated a quantum simulation that in theory goes beyond the mean-field level. We achieved chemical accuracy for small molecules.

The protocol presents significant improvements in the circuit depth and running time, key metrics for chemistry simulation. Through systematic hardware enhancements and the integration of error mitigation techniques, we push forward the limit of quantum computational chemistry and successfully scale up the implementation of VQE with an optimised unitary coupled-cluster ansatz. We produced high-precision results of the ground-state energy for molecules with error suppression by around two orders of magnitude. Details could be found [here](https://www.nature.com/articles/s41567-024-02530-z).

 
 **Quantum many-body phenomena**

I have been interested in interesting many-body phenomena since my undergraduate study. I wonder if we could have a better understanding of emergent quantum phenomena in quantum materials, especially high-temperature superconductors and magnetic materials. Some related works could be found [here](https://www.nature.com/articles/s41535-023-00604-4).



