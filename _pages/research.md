---
layout: archive
title: "Research Topics"
permalink: /research/
author_profile: true
---



I have a broad interest in quantum computing, quantum information, and quantum many-body physics. Below let us explore a few topics that I have been interested in.

Quantum computing
-----

Quantum problems can be broadly classified into two categories: static problems and dynamics problems. Static problems correspond to finding a quantum system's lowest energy state or, more generally, its eigenstate. Applications range from drug design to uncovering novel phases of matter, which, to most extent, can be transformed into an eigenstate problem. Dynamics problems include simulating the dynamics of a quantum system, for example, simulating the dynamics governed by a Hamiltonian, also known as Hamiltonian simulation. Applications include identifying dissipative phase transitions and studying information scrambling and transport.  

I have been working on improving algorithmic complexity in the two general classes of quantum problems. 

**Eigenstate problems** We have developed several quantum algorithms for finding the ground-state or excited states of a quantum system. One example is a near-optimal eigenstate preparation method, termed quantum algorithmic cooling, in collaboration with Pei and Xiao. The algorithmic cooling operates deterministically without relying on assumptions about parametrised circuits and can guarantee simulation accuracy with near-optimal query complexity in precision, gap, etc. The query complexity (of real-time evolution $$e^{-iHt}$$) matches the results by QSP and QETU, and shows an advantage over quantum phase estimation and variational methods. More details could be found [here](https://arxiv.org/abs/2109.15304).

In more recent work in collaboration with Pei, Tom and Myungshik, we provide a full-stack design of a quantum algorithm which considers the gate complexity, as opposed to previous algorithms based on querying either block encoding of the Hamiltonian and time evolution $$e^{-iHt}$$. We show that it maintains near-optimal system size and precision scaling. We compared the resource requirements (CNOT gates, T gates and qubit numbers) by state-of-the-art methods, including phase estimation, QSP, and QETU, in tasks of lattice models and molecular problems. For example, we can estimate the resources for typical complex compounds, like FeMoco and a cytochrome enzyme P450, commonly used for resource benchmarking (e.g., [paper 1](https://www.pnas.org/doi/10.1073/pnas.2203533119) and [paper 2](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.2.030305) by Google and [paper 3](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.3.033055) by Microsoft). We provided a toolbox for analysing resource requirements for these advanced methods when compiled at the gate level, which could be useful for resource estimations in the noisy intermediate-scale quantum (NISQ) and fault-tolerant quantum computing (FTQC) era. Details could be found [here](https://arxiv.org/abs/2406.04307).

**Dynamics problems**, i.e., simulating the dynamics of quantum systems, is a fundamental task in quantum physics and is believed to be a major application of quantum computers. Below, I introduce a few related works.

Perturbative approach to quantum dynamics simulation. Perturbation theory brings about great success in quantitative predictions of quantum mechanics; however, challenges remain in solving the major component and computing the power series. We addressed this challenge by developing a conceptually novel approach, perturbative quantum simulation (PQS), which exploits the complementary strength of quantum computing and perturbation theory. We demonstrated that PQS is applicable to simulate classically challenging systems, such as large systems with weak inter-subsystem interactions or intermediate systems with general interactions. Remarkably, PQS shows advantages over conventional quantum simulation algorithms concerning the quantum resource requirements and noise robustness. I have explored applications in interacting bosons, fermions, and quantum spins in different topological structures and studied different quantum phenomena on systems of up to 48 qubits, such as information propagation, charge-spin separation, magnetism, etc. Details could be found [here](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.129.120505).

Adaptive product formulae. We introduced an adaptive product formula which can produce a compact quantum circuit for Hamiltonian simulation. We introduced a measurable quantifier to describe the dynamics simulation error. The simulation error is rigorously analysed. The adaptive product formula is proven to guarantee simulation accuracy, showing an advantage over conventional product formula methods or variational quantum algorithms. Our method can be used as a subroutine of many quantum algorithms, and we demonstrated the applications for solving eigenvalue problems in quantum chemistry. Our method largely reduces quantum resources for Hamiltonian simulation and thus enables practical implementation with near-term or early fault-tolerant quantum devices. Details could be found [here](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.130.040601).

**Hybrid quantum-classical computing**
My collaborators and I have been extensively working on hybrid quantum-classical computing, such as variational quantum algorithms, which use a small quantum computer to carry out a hard-to-compute subroutine and a classical computer for optimisation ([link](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.125.010501)). With Xiao, Suguru, Ying and Simon, we proposed variational algorithms for simulating open system dynamics and general processes. An application is to simulate $$\lambda-\phi^4$$ scalar quantum field theories. We discussed the encoding of the field theory problem under different bases and in either real space or momentum space, variational state preparation, simulation of particle scattering, and resource requirements in collaboration with Junyu, Zimu, Han and Xiao. Details could be found [here](https://iopscience.iop.org/article/10.1088/2632-2153/aca06b/meta). Other applications in quantum many-body problems are discussed below.


**Quantum embedding simulation of molecules and materials**

To facilitate the practical applications of quantum computing, I have worked with industrial partners to develop quantum embedding schemes tailored to solving physical problems, particularly in the domains of quantum materials and molecules. We emulated quantum hardware classically and tested the viability of quantum simulation for quantum many-body systems. In a collaborative project with Dingshun and colleagues, we have emulated different materials, from hydrogen chains to nickel oxides, with a problem size of up to 10,000 qubits before resource reduction, which is currently the largest-scale proof-of-principle quantum simulation. They have also stimulated new directions in pushing forward the applications of quantum computing by integrating advanced classical methods. Simulations of molecules and materials can be found [here](https://pubs.rsc.org/en/content/articlehtml/2022/sc/d2sc01492k) and [here](https://www.nature.com/articles/s41524-023-01045-0).


**Quantum computing and spectroscopy**

Estimating spectral features of quantum many-body systems has attracted great attention in material science
and quantum chemistry. To achieve this task, various experimental and theoretical techniques have been developed, including spectroscopy techniques, and quantum simulation either by engineering controlled quantum
devices or executing quantum algorithms. However, probing a quantum system's behaviour is challenging and demands substantial resources for both approaches. For instance, a real probe by neutron spectroscopy requires access to large-scale facilities with high-intensity neutron beams, while quantum computing of eigenenergies, such as phase estimation, typically requires a long coherence time in engineering controlled quantum devices. In a recent project, we established a framework for probing the excitation spectrum of quantum many-body systems with quantum simulators. More details could be found [here](https://arxiv.org/abs/2305.07649).

I have been thinking of the crossover between static problems and dynamics problems, well-established spectroscopy techniques and quantum computing, and many seemingly different subjects. Some philosophical discussions on the notion of quantum machine, quantum simulation and spectroscopy can be found in my [thesis](https://ora.ox.ac.uk/objects/uuid:de5499cb-9c49-4be3-acc1-5be4cb81099d).


Quantum error mitigation and its transitions to quantum error correction
-----

To effectively demonstrate the utility of quantum computing, we must confront challenges associated with the practical use of noisy quantum computers. Errors are an inherent aspect of quantum computing. Ensuring that quantum computing delivers accurate results in the presence of these errors is a critical consideration. Together with Suguru, Xiao, Vlatko and Simon, we initially proposed new QEM schemes to mitigate realistic noise described by Lindbladian appearing in both digital and analogue quantum devices. For noise from imperfections of the engineered Hamiltonian or additional noise operators, we showed it can be effectively suppressed by a new QEM method, termed stochastic QEM. Our method only requires accurate single qubit controls, and is thus applicable to all digital quantum computers and various analogue simulators. Details could be found [here](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.15.034026).

I have been wondering how to overcome the fundamental limits set up by QEM. This motivates us to think about an intermediate form between QEM and QEC. In recent work, we introduced an information-theoretic machinery, a commutation-derived quantum filter, to purify or correct quantum channels. This addresses the sampling problem in QEM.


Quantum computational chemistry
-----

The application of quantum computing to computational chemistry faces various experimental and theoretical challenges. In a recent project with USTC and Peking, we addressed the critical challenges associated with solving molecular electronic structures using noisy quantum processors. We demonstrated a quantum simulation that in theory goes beyond the mean-field level. 

The protocol presents significant improvements in the circuit depth and running time, key metrics for chemistry simulation. Through systematic hardware enhancements and the integration of error mitigation techniques, we push forward the limit of quantum computational chemistry and successfully scale up the implementation of VQE with an optimised unitary coupled-cluster ansatz. We produced high-precision results of the ground-state energy for molecules with error suppression by around two orders of magnitude; remarkably, we achieved chemical accuracy for small molecules. Details could be found [here](https://www.nature.com/articles/s41567-024-02530-z).

Apart from the circuit generation method developed in this work, fast quantum state measurement is crucial. This leverages the overlapped grouping method developed [here](https://quantum-journal.org/papers/q-2023-01-13-896/) and [here](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.200501). Interestingly, the current advanced measurment schemes, like the classical shadow method and its variants (derandomised shadow and adaptive shadow), can be understood in the framework presented in the [paper](https://quantum-journal.org/papers/q-2023-01-13-896/) and [paper](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.127.200501)

 
Quantum many-body phenomena
-----

I have been interested in interesting many-body phenomena since my undergraduate study. I wonder if we could have a better understanding of emergent quantum phenomena in quantum materials, especially high-temperature superconductors and magnetic materials. In my undergraduate thesis, I explored the microscopic origin of electronic nematic order in iron-selenide-based superconductors advised by Yuan Li. Please email me if you are interested in my undergraduate work. Some related works could be found [here](https://www.nature.com/articles/s41535-023-00604-4) and [here](https://www.sciencedirect.com/science/article/abs/pii/S209592731730628X).



