# Memristive SNN - Privacy - Model Inversion and Fault Injection Attack

This repository contains the reference implementation for our research on *Fault Injection* and *Model Inversion* attacks targeting **Spiking Neural Networks (SNNs)** deployed on neuromorphic or memristive-inspired platforms. The project investigates how device-level perturbations and inversion-based reconstruction methods compromise the confidentiality, integrity, and robustness of SNN-driven systems.

---

## 1. Overview

Spiking Neural Networks are increasingly adopted in low-power and event-driven computing. Despite their advantages, their security properties remain underexplored. This repository provides:

- Fault Injection methods (with memristive perturbations).
- Model Inversion attacks adapted to temporally coded SNN outputs.
- Baseline, quantized, and memristive-inspired SNN models.
- Evaluation pipelines for leakage quantification and robustness analysis.

The implementation emphasizes reproducibility and modularity for security and privacy research.

---

## 2. Key Contributions

- Device-aware SNN simulation with configurable synaptic update rules.
- Practical fault injection primitives targeting:
  - Membrane potential dynamics  
  - Synaptic weights  
  - Spike train propagation  
  - Device-level noise (e.g., memristor switching variability)
- Gradient-based and optimization-driven model inversion tailored to SNNs.
- Benchmarks various datasets.
- Leakage and robustness metrics specifically designed for neuromorphic architectures.

---

## 3. Requirements

- Python 3.10+
- PyTorch  
- snnTorch  
- NumPy, SciPy, Matplotlib  
- (Optional) IBM aihwkit for physical-device simulation

Install dependencies

---

## 4. Datasets

Supported datasets include:

- MNIST
- Fashion-MNIST
- AT & T Faces
- DVS Gesture 

---

## 5. Evaluation Metrics

- Classification accuracy
- Fault-induced misclassification rate
- Reconstruction similarity (SSIM, PSNR, MSE)
- Temporal leakage surfaces
- Robustness curves under injection intensity

Visualization utilities are included.
---





