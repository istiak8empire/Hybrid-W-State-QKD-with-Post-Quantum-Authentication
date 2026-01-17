# 🌌 Quantum-Safe Cryptography Meets Practical Implementation

**A Hybrid W-State Quantum Key Distribution and Post-Quantum Authentication Scheme for Secure AES Encryption**

[![Python]](https://www.python.org/downloads/)
[![Qiskit](https://img.shields.io/badge/Built%20with-Qiskit-6929C4.svg)](https://qiskit.org/)
[![Post-Quantum](https://img.shields.io/badge/Post--Quantum-NIST%20Standardized-green.svg)](https://csrc.nist.gov/projects/post-quantum-cryptography)
[![arXiv](https://img.shields.io/badge/arXiv-XXXX.XXXXX-b31b1b.svg)](https://arxiv.org/abs/XXXX.XXXXX)

## ✨ At a Glance

> **Exploring how quantum and post-quantum cryptography can be combined to strengthen secure key establishment in future communication systems.**
This repository presents a **research-oriented, open-source implementation** of a hybrid cryptographic framework that integrates:

🔮 **Quantum Key Distribution** using noise-resilient W-states  
🔐 **Post-Quantum Authentication** via NIST-standardized CRYSTALS-Dilithium and generate pre-key using it 

⚡ **Encryption using AES-256-GCM** with secret key achieved from our hybrid key distribution protocol

The framework focuses on **protecting the key establishment and authentication layers**, which are known to be vulnerable to quantum adversaries, while leveraging AES as a robust symmetric cipher for payload encryption.

---

## 🚀 Why This Matters

| The Problem | Our Solution |
|-------------|-------------|
| ❌ **Quantum computers will break RSA/ECC** within 10-20 years | ✅ **Quantum-safe today** with lattice-based cryptography |
| ❌ **Traditional QKD post-processing fails** to generate identical keys due to noise and particle loss | ✅ **W states survives with proposed entanglement verification method** where GHZ states fail in case of multipartite entanglement |
| ❌ **Most solutions** are either quantum OR classical | ✅ **True hybrid architecture** that leverages the best of both worlds |
| ❌ **Theoretical papers** without working code | ✅ **Implementation validated by simulations** you can run right now |

---

## 🏗️ System Architecture (High-Level)



### **Quantum Layer**
* W-state preparation and distribution.
* Decoy photon insertion for eavesdropping detection.
* Measurement, key extraction, and entanglement verification.

### **Classical Authentication Layer**
* Dilithium-based message signing.
* Secure classical channel establishment.
* Pre-key derivation from signed session data.

### **Encryption Layer**
* AES-256 encryption using quantum-derived keys.
* Performance benchmarking across different AES modes (CBC, GCM, etc.).


---
## 🧪 Experimental Results
The system was validated under ideal and noisy quantum channels. Key metrics evaluated include:

* **Quantum Bit Error Rate (QBER):** Analysis of error thresholds under decoherence.
* **Key Generation Success Rate:** Efficiency of the W-state protocol.
* **Noise Robustness:** Resilience comparison against standard Bell-state protocols.
* **Performance Overhead:** Latency analysis of AES encryption and Post-Quantum signature verification.

**Conclusion:** The results demonstrate that the proposed hybrid scheme remains secure, efficient, and practical even under realistic quantum noise conditions.
---
