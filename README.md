# 📌 Developing Game-Theoretic Models for Quantum Resource Allocation in Cloud-Enabled Distributed Quantum Computing

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Research](https://img.shields.io/badge/Type-Research-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Under%20Review-yellow)

---

## 📚 Table of Contents

* [Abstract](#-abstract)
* [Keywords](#-keywords)
* [Research Contributions](#-research-contributions)
* [System Model](#-system-model)
* [Methodology](#-methodology)
* [Experimental Setup](#-experimental-setup)
* [Results & Analysis](#-results--analysis)
* [Implementation](#-implementation)
* [Reproducibility](#-reproducibility)
* [Applications](#-applications)
* [Future Work](#-future-work)
* [Citation](#-citation)
* [Author](#-author)
* [License](#-license)

---

## 📖 Abstract

Distributed Quantum Computing (DQC) enables scalable quantum processing by interconnecting geographically distributed quantum processors through cloud infrastructures. However, efficient allocation of limited quantum resources—such as qubits, execution slots, and entanglement links—remains a fundamental challenge due to decoherence, noise, and hardware constraints.

This work presents a **game-theoretic framework for incentive-aware quantum resource allocation** in multi-user cloud-enabled DQC environments. By modeling users as rational agents in a non-cooperative setting, the proposed approach achieves improved fairness, faster convergence, and enhanced system-wide utility under realistic quantum constraints.

---

## 🔑 Keywords

Quantum Resource Allocation, Distributed Quantum Computing, Game Theory, Nash Equilibrium, Quantum Cloud, Multi-user Systems, Optimization

---

## 🎯 Research Contributions

* Novel formulation of **quantum resource allocation as a strategic non-cooperative game**
* Design of **quantum-aware utility functions** incorporating fidelity, decoherence, and entanglement cost
* Development and comparison of:

  * Quantum Best Response Dynamics (QBRD)
  * Iterative Convergence with Equilibrium Dynamics (ICED)
  * Classical Nash-Based Algorithm (CNBA)
  * Hybrid Quantum-Classical Approach (HQCA)
* Demonstration of:

  * **2–6× convergence speedup**
  * **Near-linear social welfare scaling**
  * **Improved fairness in multi-user environments**
* Alignment with **NISQ-era quantum system constraints**

---

## 🧠 System Model

* **Players:** Multiple users requesting quantum resources
* **Strategies:** Allocation of qubits, circuits, execution time
* **Objective:** Maximize individual utility while ensuring system-wide efficiency

**Utility Function:**

```id="sysu12"
U_i = f(Q_i, F_i, D_i, E_i)
```

Where:

* `Q_i` → Allocated qubits
* `F_i` → Gate fidelity
* `D_i` → Decoherence factor
* `E_i` → Entanglement cost

---

## ⚙️ Methodology

1. **Initialization**

   * Define system constraints and resource pool

2. **Game Formulation**

   * Construct payoff functions incorporating quantum parameters

3. **Strategy Update**

   * Apply iterative dynamics (QBRD / ICED)

4. **Equilibrium Computation**

   * Identify Nash equilibrium / Pareto-optimal allocation

5. **Performance Evaluation**

   * Convergence speed
   * Resource utilization
   * Fairness metrics

---

## 📊 Experimental Setup

* **Simulation Type:** Classical simulation of quantum systems
* **Platform:** Python (Jupyter Notebook)
* **Workload:** Synthetic multi-user demand model
* **Evaluation Metrics:**

  * Convergence iterations
  * Allocation efficiency
  * Social welfare
  * Noise robustness

---

## 📈 Results & Analysis

### 🔹 Convergence Performance

![Convergence](<img width="1615" height="616" alt="fig5_resource_alloc" src="https://github.com/user-attachments/assets/8c4aff28-8a0d-406f-b2fc-31d72cea0cfd" />
<img width="1035" height="660" alt="fig3_convergence" src="https://github.com/user-attachments/assets/163a980f-dca2-4907-ba2f-7c7348903478" />
)

### 🔹 Resource Allocation Efficiency

![Allocation](![Uploading fig5_resource_alloc.png…]()
)

### 🔹 Social Welfare Scaling

![Welfare](<img width="1034" height="660" alt="fig10_social_welfare" src="https://github.com/user-attachments/assets/d0e66f99-3c53-46e3-94d6-62fee4710e9e" />
)

### 🔹 Noise Robustness

![Noise](<img width="1034" height="660" alt="fig11_noise_robustness" src="https://github.com/user-attachments/assets/12220ac9-7067-4f13-a9d1-9a04c86fe187" />
)

---

### 📊 Result Summary Table

| Algorithm | Convergence Speed | Iterations | Social Welfare     | Fairness | Noise Robustness |
| --------- | ----------------- | ---------- | ------------------ | -------- | ---------------- |
| **QBRD**  | Very Fast         | ~1–2       | High               | High     | Moderate         |
| **ICED**  | Fast              | ~10        | High               | High     | High             |
| **CNBA**  | Moderate          | ~15        | Very High (Pareto) | Moderate | Moderate         |
| **HQCA**  | Slow              | >15        | Adaptive           | High     | Very High        |

---

### 📌 Key Insights

* QBRD achieves **fastest convergence**
* ICED provides **stable equilibrium behavior**
* CNBA ensures **Pareto optimality**
* HQCA offers **robust adaptability to quantum noise**
* Overall system achieves **near-linear scalability in social welfare**

---

## 🧪 Implementation

### 📂 Repository Structure

```id="repo45"
├── Quantum game theory DQC obj1.ipynb
├── figures/
│   ├── fig3_convergence.png
│   ├── fig5_resource_alloc.png
│   ├── fig10_social_welfare.png
│   ├── fig11_noise_robustness.png
├── README.md
```

---

## ⚙️ Requirements

```bash id="req12"
pip install numpy pandas matplotlib
```

(Optional)

```bash id="req34"
pip install qiskit
```

---

## 🚀 How to Run

```bash id="run78"
git clone https://github.com/mahantapabani-lgtm/quantum-geme-theory-DQC.git
cd quantum-geme-theory-DQC
jupyter notebook
```

Run:

```id="run99"
Quantum game theory DQC obj1.ipynb
```

---

## 🔬 Reproducibility

* Synthetic dataset generation included in notebook
* Deterministic initialization for fair comparison
* All experiments reproducible via provided code

---

## 📌 Applications

* Quantum Cloud Computing
* Multi-user Quantum Systems
* Quantum Network Scheduling
* Resource Optimization in NISQ devices

---

## 🔮 Future Work

* Deployment on real quantum hardware (IBM Quantum, IonQ)
* Integration with reinforcement learning
* Multi-objective optimization (latency, fidelity, energy)
* Extension to quantum internet architectures

---

## 👩‍💻 Author

**Pabani Mahanta**
GitHub: https://github.com/mahantapabani-lgtm

---

## 📜 License

MIT License

---

## ⭐ Acknowledgment

This work contributes toward advancing efficient and scalable quantum resource management in next-generation distributed quantum computing systems.
