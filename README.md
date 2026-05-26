<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a14,40:0d1225,70:1a1a3e,100:2a1a3e&height=200&section=header&text=Malhar%20Pangarkar&fontSize=54&fontColor=b8c5d6&fontAlignY=42&desc=I%20have%20tried%20to%20be%20what%20you%20wanted.%20I%20am%20what%20I%20am.&descAlignY=62&descSize=13&animation=fadeIn" width="100%"/>

</div>

<div align="center">

[![](https://img.shields.io/badge/pip%20install%20nato--opt-PyPI-0d0d1f?style=flat-square&labelColor=0d0d1f&color=4a3f6b)](https://pypi.org/project/nato-opt/)
[![](https://img.shields.io/badge/malharpangarkar08%40gmail.com-contact-0d0d1f?style=flat-square&labelColor=0d0d1f&color=4a3f6b)](mailto:malharpangarkar08@gmail.com)

</div>

---

## Published

### [NATO — Neural Adaptive Training Optimizer](https://github.com/Malhar1912/NATO)
`pip install nato-opt` · co-authored with Atharva Khambete · GPU/CUDA · MIT

A custom PyTorch optimizer with three original regularization techniques, all built on existing forward passes — zero extra compute overhead.

| Technique | What it does |
|---|---|
| **Fourier Spectral Penalty** | Regularises model weights in frequency space, not weight space |
| **Kakeya Directional Penalty** | Penalises gradient-direction consistency — forces exploratory updates |
| **N-D FFT Gradient Filtering** | Low-pass filters the gradient signal before every optimizer step |

```python
from nato_opt import NATOOptimizer, fourier_spectral_penalty, low_pass_filter_gradients

optimizer = NATOOptimizer(model.parameters(), lr=1e-3)
fsp       = fourier_spectral_penalty(model, lambda_fsp=1e-6)
low_pass_filter_gradients(model, cutoff_ratio=0.5)
optimizer.step(epoch)
```

[![PyPI](https://img.shields.io/pypi/v/nato-opt?style=flat-square&labelColor=0d0d1f&color=4a3f6b&logo=pypi&logoColor=b8c5d6)](https://pypi.org/project/nato-opt/)
![](https://img.shields.io/badge/python-3.8+-2d2d4a?style=flat-square)
![](https://img.shields.io/badge/CUDA-accelerated-0d1a0d?style=flat-square&logo=nvidia&logoColor=76b900)

---

## Manuscripts

### [GeoSDE-IDS — Geometric Stochastic Differential Intrusion Detection](https://github.com/Malhar1912/GeoSDE-IDS)
Full Elsevier manuscript · CIC-IDS 2017 · NSL-KDD · UNSW-NB15 · 5 seeds · reproducibility checklist

An IDS that models network traffic on **hyperbolic manifolds** (Poincaré Ball + Lorentz), using Neural SDEs to learn normal traffic dynamics — anomalies detected as geometric distortions in curved space, not threshold violations.

Five detection signals running in parallel:
- **Ollivier-Ricci Curvature** distortion
- **Dirichlet Energy Functional** acceleration
- **Möbius Invariance** violation
- **Fokker-Planck Density** evolution via KL-Divergence
- **SDE Drift** deviation

Signals fused via meta-classifier (LR + MLP). LaTeX manuscript, benchmark CSVs, and figure generation scripts all committed.

![](https://img.shields.io/badge/Python%20·%20TeX%20·%20Elsevier-manuscript-2d2d4a?style=flat-square)
![](https://img.shields.io/badge/3%20datasets%20·%205%20seeds-reproduced-4a3f6b?style=flat-square)

---

### [TCR — Threshold-Constrained Replay Framework](https://github.com/Malhar1912/Threshold-Constrained-Replay-TCR-A-Constrained-Multi-Objective-Replay-Framework)
RL research paper in progress · 7-phase formal specification · ablation protocols · validation gates

Reframes experience replay as a **constrained stochastic resource allocation problem** — not a ranking problem. The core objective:

$$\max_{q \in \Delta}\ \mathbb{E}_{\tau \sim q}\bigl[\Delta\mathcal{L}(\tau)\bigr] \quad \text{s.t.} \quad \mathrm{KL}(q\,\|\,p) \le \varepsilon,\quad |D^*| \le B$$

Phase 0.4 is a mandatory validation gate — ρ > 0.3, p < 0.05, across ≥80% of environments — before any subsequent phase proceeds. Benchmarks against PER, DreamerV3, and Uniform Replay on Atari-100k, DMC, and Procgen.

![](https://img.shields.io/badge/reinforcement%20learning-constrained%20optimization-2d2d4a?style=flat-square)
![](https://img.shields.io/badge/status-in%20progress-4a3f6b?style=flat-square)

---

## Formal Methods

### [SAT Solver — DPLL with Live Decision Tree Visualization](https://github.com/Malhar1912/SAT_Solver)
Full DPLL implementation with unit propagation and pure literal elimination. Random k-CNF generator for stress testing. Real-time decision tree rendered via `networkx` + `matplotlib` — green nodes for satisfiable paths, red for conflict. The algorithm made visible.

`Python` · `MIT`

### [Halting Problem Simulation](https://github.com/Malhar1912/Halting_Problem_Simulation) · [↗ Live](https://halting-problem-simulation.vercel.app)
Interactive formal proof of undecidability. Animated REBEL paradox walkthrough. Step-by-step contradiction. Academic references to Turing, Church, and Gödel. Cyberpunk React app, deployed.

`TypeScript` · `Framer Motion` · `Vercel`

---

## Deployed

| Project | Description | Stack |
|---|---|---|
| [Q-Shield](https://github.com/Malhar1912/Q-Shield-Quaternionic-Key-Exchange-Explorer) · [↗](https://q-shield-quaternionic-key-exchange.vercel.app) | Post-quantum key exchange explorer built on quaternion algebra — ℍ-based cryptographic primitives beyond standard ECC | TypeScript · Vercel |
| [LT-Graph](https://github.com/Malhar1912/LT-Graph) · [↗](https://lt-graph.vercel.app) | Interactive graph traversal toolkit with simulation layer and Gemini API integration | TypeScript · Vite |

---

## Stack

<div align="center">

![](https://img.shields.io/badge/Python-0d0d1f?style=for-the-badge&logo=python&logoColor=b8c5d6)
![](https://img.shields.io/badge/TypeScript-0d0d1f?style=for-the-badge&logo=typescript&logoColor=b8c5d6)
![](https://img.shields.io/badge/PyTorch-0d0d1f?style=for-the-badge&logo=pytorch&logoColor=b8c5d6)
![](https://img.shields.io/badge/React-0d0d1f?style=for-the-badge&logo=react&logoColor=b8c5d6)
![](https://img.shields.io/badge/C++-0d0d1f?style=for-the-badge&logo=cplusplus&logoColor=b8c5d6)
![](https://img.shields.io/badge/Rust-0d0d1f?style=for-the-badge&logo=rust&logoColor=b8c5d6)
![](https://img.shields.io/badge/LaTeX-0d0d1f?style=for-the-badge&logo=latex&logoColor=b8c5d6)
![](https://img.shields.io/badge/CUDA-0d0d1f?style=for-the-badge&logo=nvidia&logoColor=76b900)

</div>

---

## Stats

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=Malhar1912&show_icons=true&hide_border=true&bg_color=0a0a14&title_color=b8c5d6&icon_color=4a3f6b&text_color=7a8fa6&include_all_commits=true&count_private=true"/>
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Malhar1912&layout=compact&langs_count=7&hide_border=true&bg_color=0a0a14&title_color=b8c5d6&text_color=7a8fa6&hide=html,css"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Malhar1912&hide_border=true&background=0a0a14&dates=4a5568&ring=4a3f6b&fire=7a8fa6&currStreakNum=b8c5d6&sideNums=b8c5d6&currStreakLabel=7a8fa6&sideLabels=7a8fa6)](https://git.io/streak-stats)

</div>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2a1a3e,50:1a1a3e,100:0a0a14&height=120&section=footer&animation=fadeIn" width="100%"/>

![](https://komarev.com/ghpvc/?username=Malhar1912&color=4a3f6b&style=flat-square&label=)
</div>
