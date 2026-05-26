<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,25:080820,60:130d35,100:1e0a4a&height=220&section=header&text=Malhar%20Pangarkar&fontSize=64&fontColor=ffffff&fontAlignY=38&desc=research.%20systems.%20theory.&descAlignY=60&descSize=18&animation=fadeIn" width="100%"/>

</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=19&pause=1100&color=C084FC&center=true&vCenter=true&width=700&lines=Published+PyPI+package+%E2%80%94+nato-opt+%F0%9F%93%A6;Elsevier+paper+%E2%80%94+hyperbolic+manifold+IDS+%F0%9F%93%84;RL+research+%E2%80%94+constrained+multi-objective+replay+%F0%9F%A7%A0;Formal+methods+%E2%80%94+SAT+solver+%2B+Halting+Problem+%E2%9A%96%EF%B8%8F;Post-quantum+crypto+%E2%80%94+quaternion+key+exchange+%F0%9F%94%90)](https://git.io/typing-svg)

</div>

---

## ⚡ `whoami`

```python
malhar = {
    "name"       : "Malhar Pangarkar",
    "alias"      : "Malhar1912",
    "email"      : "malharpangarkar08@gmail.com",
    "domains"    : [
        "Deep Learning Optimization",
        "Reinforcement Learning (theory + systems)",
        "Post-Quantum Cryptography",
        "Computational Complexity & Formal Methods",
        "Geometric/Stochastic Methods for Security",
    ],
    "output_type": ["PyPI packages", "Elsevier manuscripts", "deployed apps", "RL frameworks"],
    "philosophy" : "Build at the edge of tractability. Formalize before you implement.",
}
```

---

## 🏆 Projects — Ranked by Depth & Originality

---

### 🥇 [NATO — Neural Adaptive Training Optimizer](https://github.com/Malhar1912/NATO)

[![PyPI](https://img.shields.io/pypi/v/nato-opt?color=7c3aed&style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/nato-opt/)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-a855f7?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![CUDA](https://img.shields.io/badge/CUDA-accelerated-76b900?style=flat-square&logo=nvidia&logoColor=white)](https://developer.nvidia.com/cuda-toolkit)
[![License: MIT](https://img.shields.io/badge/license-MIT-6d28d9?style=flat-square)](https://opensource.org/licenses/MIT)

> **`pip install nato-opt`** — a published, installable PyTorch optimizer. Co-authored with Atharva Khambete.

Three original regularization techniques, all operating on top of existing forward passes — zero added overhead:

| Technique | Mechanism |
|---|---|
| **Fourier Spectral Penalty (FSP)** | Regularizes model weights in the frequency domain, penalizing high-frequency components |
| **Kakeya Directional Penalty** | Penalizes gradient-direction consistency — forces exploratory, diverse updates |
| **N-D FFT Gradient Filtering** | Low-pass filters gradients before the optimizer step; smooths high-frequency noise |

```python
from nato_opt import NATOOptimizer, fourier_spectral_penalty, low_pass_filter_gradients

optimizer = NATOOptimizer(model.parameters(), lr=1e-3)
fsp = fourier_spectral_penalty(model, lambda_fsp=1e-6)
low_pass_filter_gradients(model, cutoff_ratio=0.5)
optimizer.step(epoch)
```

`Python` · `PyTorch` · `Signal Processing` · `Optimization` · `GPU / CUDA`

---

### 🥈 [GeoSDE-IDS — Geometric Stochastic Differential Intrusion Detection](https://github.com/Malhar1912/GeoSDE-IDS)

> Full Elsevier manuscript (`paper/elsevier_manuscript.tex`). Benchmarked on CIC-IDS 2017, NSL-KDD, UNSW-NB15 across 5 seeds.

An IDS that abandons Euclidean space entirely — instead modeling network flow dynamics on **hyperbolic manifolds** (Poincaré Ball + Lorentz/Hyperboloid) via Neural SDEs, exploiting the natural hierarchical structure of network graphs.

**5-signal detection engine:**
- Ollivier-Ricci Curvature distortion
- Dirichlet Energy Functional acceleration
- Möbius Invariance violation
- Fokker-Planck Density evolution (KL-Divergence)
- SDE Drift Deviation

Signals fused via meta-classifier (LR + MLP). Full reproducibility checklist, `results/` CSVs committed, LaTeX figures auto-generated from `src/scripts/generate_figures.py`.

`Python` · `PyTorch` · `Differential Geometry` · `Neural SDEs` · `Network Security` · `TeX`

---

### 🥉 [TCR — Threshold-Constrained Replay Framework](https://github.com/Malhar1912/Threshold-Constrained-Replay-TCR-A-Constrained-Multi-Objective-Replay-Framework)

> Research paper in progress. 7-phase formal specification with LaTeX math, ablation protocols, and validation gates.

Reframes experience replay as a **constrained stochastic resource allocation problem** — not just a ranking problem. Solves:

$$\max_{q \in \Delta}\ \mathbb{E}_{\tau \sim q}[\Delta \mathcal{L}(\tau)] \quad \text{s.t.} \quad \text{KL}(q \| p) \le \epsilon,\quad |D^*| \le B$$

Includes proxy validation gates (Phase 0.4 must pass: ρ > 0.3, p < 0.05 across 80% of envs), async actor-learner pipeline, IS-weighted gradient correction, and failure-mode safeguards. Benchmarks against PER, DreamerV3, and Uniform Replay on Atari-100k, DMC, and Procgen.

`Python` · `Reinforcement Learning` · `Constrained Optimization` · `Research`

---

### 4️⃣ [SAT_Solver — DPLL with Live Decision Tree Visualization](https://github.com/Malhar1912/SAT_Solver)

Full DPLL implementation — unit propagation, pure literal elimination, random k-CNF generator — with a real-time decision tree rendered via `networkx` + `matplotlib`. Green nodes = satisfiable paths. Red = conflict/backtrack. The algorithm made *visible*.

`Python` · `Formal Methods` · `Visualization` · `MIT License`

---

### 5️⃣ [Halting Problem Simulation](https://github.com/Malhar1912/Halting_Problem_Simulation) · 🌐 [Live Demo](https://halting-problem-simulation.vercel.app)

An interactive proof of undecidability — animated, cyberpunk-styled React app. Walks through the REBEL program paradox step-by-step with formal proof, academic references (Turing, Church, Gödel), and an AGI-implications section. The kind of thing you send someone when they ask "why can't we just verify all programs?"

`TypeScript` · `React` · `Framer Motion` · `Tailwind` · `Vercel`

---

### 6️⃣ [Q-Shield — Quaternionic Key Exchange Explorer](https://github.com/Malhar1912/Q-Shield-Quaternionic-Key-Exchange-Explorer) · 🌐 [Live Demo](https://q-shield-quaternionic-key-exchange.vercel.app)

Post-quantum key exchange built on **quaternion algebra** — exploring ℍ-based primitives beyond standard lattice/ECC approaches. Interactive TypeScript/React explorer deployed to production.

`TypeScript` · `Post-Quantum Cryptography` · `Abstract Algebra` · `Vercel`

---

### 7️⃣ [LT-Graph](https://github.com/Malhar1912/LT-Graph) · 🌐 [Live Demo](https://lt-graph.vercel.app)

Interactive graph theory toolkit with a simulation layer and Gemini API integration. Full TypeScript/React, test suite included.

`TypeScript` · `Graph Theory` · `Gemini API` · `Vite`

---

## 🛠️ Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![LaTeX](https://img.shields.io/badge/LaTeX-008080?style=for-the-badge&logo=latex&logoColor=white)

</div>

---

## 📊 Stats

<div align="center">

<img height="175em" src="https://github-readme-stats.vercel.app/api?username=Malhar1912&show_icons=true&theme=midnight-purple&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=c084fc&icon_color=a855f7&text_color=e2e8f0"/>
<img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Malhar1912&layout=compact&langs_count=7&theme=midnight-purple&hide_border=true&bg_color=0d1117&title_color=c084fc&text_color=e2e8f0&hide=html,css"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Malhar1912&theme=midnight-purple&hide_border=true&background=0d1117&dates=9ca3af&ring=7C3AED&fire=C4B5FD&currStreakNum=ffffff&sideNums=ffffff&currStreakLabel=c084fc&sideLabels=c084fc)](https://git.io/streak-stats)

</div>

---

## 📬 Contact

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Malhar1912-181717?style=for-the-badge&logo=github)](https://github.com/Malhar1912)
[![Email](https://img.shields.io/badge/Email-malharpangarkar08@gmail.com-9333ea?style=for-the-badge&logo=gmail&logoColor=white)](mailto:malharpangarkar08@gmail.com)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e0a4a,50:130d35,100:000000&height=120&section=footer&animation=fadeIn" width="100%"/>

*"The best proof is the one that makes the impossibility obvious."*

![Profile Views](https://komarev.com/ghpvc/?username=Malhar1912&color=7c3aed&style=flat-square&label=profile+views)

</div>
