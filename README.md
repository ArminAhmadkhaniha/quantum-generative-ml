# Quantum Generative Adversarial Networks (qGAN) & EQ-GAN

[![DOI: Nature](https://img.shields.io/badge/DOI-10.1038%2Fs41534--019--0223--2-blue)](https://www.nature.com/articles/s41534-019-0223-2)
[![DOI: PRL](https://img.shields.io/badge/DOI-10.1103%2FPhysRevLett.128.220505-red)](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.128.220505)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

## Overview

This repository contains independent reimplementations and performance analyses of two landmark papers in Quantum Machine Learning. The project explores the capabilities of Quantum Generative Adversarial Networks (qGANs) for efficient state loading and error mitigation.

The implementations utilize **PennyLane**, **Qiskit**, and **TorchQuantum** to reproduce the key findings of the original authors.

## Implemented Papers

### 1. qGAN for Learning and Loading Random Distributions
**Original Paper:** *Quantum Generative Adversarial Networks for learning and loading random distributions* (Zoufal et al., Nature npj Quantum Information, 2019).

* **Goal:** Efficiently load classical probability distributions into quantum states using a hybrid quantum-classical GAN.
* **Key Result Reproduced:** Demonstrated that the network can learn a representation of the probability distribution with $O(poly(n))$ gates, enabling efficient amplitude estimation.
* **Code:** Located in `qgan_distribution/`.

### 2. Entangling Quantum GANs (EQ-GAN)
**Original Paper:** *Entangling Quantum Generative Adversarial Networks* (Anschuetz et al., Phys. Rev. Lett., 2022).

* **Goal:** Overcome standard qGAN limitations by using an "Entangling" architecture that converges to a Nash equilibrium.
* **Key Result Reproduced:** Used the EQ-GAN architecture to mitigate uncharacterized errors in quantum data generation.
* **Code:** Located in `eqgan_entangling/`.

### Installation
To install dependencies:
```bash
pip install -r requirements.txt

```