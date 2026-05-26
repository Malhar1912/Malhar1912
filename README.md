<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,30:0a0a2e,70:1a0a3e,100:2d1b69&height=220&section=header&text=Malhar%20Pangarkar&fontSize=62&fontColor=ffffff&fontAlignY=38&desc=researcher.%20builder.%20optimizer.&descAlignY=60&descSize=20&animation=fadeIn" width="100%"/>

</div>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=20&pause=1200&color=C084FC&center=true&vCenter=true&width=650&lines=Published+PyPI+package+%40+nato-opt+%F0%9F%93%A6;SAT+Solver+with+live+decision+tree+viz+%F0%9F%8C%B3;Post-quantum+crypto+in+quaternion+algebra+%F0%9F%94%90;If+NP-hard+is+easy%2C+find+a+harder+problem+%E2%9A%96%EF%B8%8F)](https://git.io/typing-svg)

</div>

---

## ⚡ `whoami`

```python
malhar = {
    "name"      : "Malhar Pangarkar",
    "alias"     : "Malhar1912",
    "focus"     : [
        "Optimization Theory",
        "Post-Quantum Cryptography",
        "Formal Methods & SAT Solving",
        "Signal Processing (FFT / Spectral Methods)",
        "Graph Algorithms & Visualization",
    ],
    "ships"     : "production code, PyPI packages, deployed apps — not just notebooks",
    "philosophy": "Build things at the edge of what's tractable. Then push the edge.",
}
```

---

## 🏆 Featured Projects

> Ranked by depth, originality, and real-world impact

---

### 🥇 [NATO — Neural Adaptive Training Optimizer](https://github.com/Malhar1912/NATO)

[![PyPI](https://img.shields.io/pypi/v/nato-opt?color=9333ea&style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/nato-opt/)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-8b5cf6?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/license-MIT-a855f7?style=flat-square)](https://opensource.org/licenses/MIT)
[![CUDA](https://img.shields.io/badge/CUDA-accelerated-76b900?style=flat-square&logo=nvidia&logoColor=white)](https://developer.nvidia.com/cuda-toolkit)

> **`pip install nato-opt`** — a real, published, installable PyPI package.

A custom PyTorch optimizer co-authored with Atharva Khambete, featuring three original regularization techniques:

| Technique | What it does |
|-----------|-------------|
| **Fourier Spectral Penalty (FSP)** | Regularization in the *frequency domain* — penalizes high-frequency weight components |
| **Kakeya Directional Penalty** | Penalizes gradient directions that are too consistent, forcing exploratory updates |
| **N-D FFT Gradient Filtering** | Low-pass filters gradients before the optimizer step to smooth high-frequency noise |

```python
from nato_opt import NATOOptimizer, fourier_spectral_penalty, low_pass_filter_gradients

optimizer = NATOOptimizer(model.parameters(), lr=1e-3)
fsp = fourier_spectral_penalty(model, lambda_fsp=1e-6)
low_pass_filter_gradients(model, cutoff_ratio=0.5)
optimizer.step(epoch)
```

`Python` · `PyTorch` · `Signal Processing` · `Optimization Research` · `GPU / CUDA`

---

### 🥈 [SAT_Solver — DPLL with Live Decision Tree Visualization](https://github.com/Malhar1912/SAT_Solver)

A full implementation of the classical **DPLL (Davis–Putnam–Logemann–Loveland)** algorithm, enhanced with:

- **Unit propagation** and **pure literal elimination** heuristics
- **Random k-CNF formula generator** for stress testing
- **Real-time decision tree visualization** via `networkx` + `matplotlib`  
  — green nodes = satisfiable paths, red nodes = conflict/backtrack points
- Modular architecture: `cnf_generator`, `sat_helpers`, `dpll_solver`, `visualization` all separated cleanly

This is what formal methods education should look like: the algorithm made *visible*.

`Python` · `Formal Methods` · `Graph Visualization` · `Algorithms`

---

### 🥉 [Q-Shield — Quaternionic Key Exchange Explorer](https://github.com/Malhar1912/Q-Shield-Quaternionic-Key-Exchange-Explorer)

🌐 **[Live Demo →](https://q-shield-quaternionic-key-exchange.vercel.app)**

An interactive explorer for post-quantum cryptographic key exchange built on **quaternion algebra** — going beyond standard lattice or ECC approaches to investigate ℍ-based key exchange primitives.

Full TypeScript/React app with a `components/`, `services/`, `utils/` architecture, shipped to production on Vercel.

`TypeScript` · `Post-Quantum Cryptography` · `Abstract Algebra` · `React` · `Vercel`

---

### 🔷 [LT-Graph — Live Graph Theory Toolkit](https://github.com/Malhar1912/LT-Graph)

🌐 **[Live Demo →](https://lt-graph.vercel.app)**

An interactive graph exploration and traversal app powered by the **Gemini API**, built with TypeScript/React and deployed to production. Simulation layer, component architecture, and full test suite included.

`TypeScript` · `Graph Theory` · `Gemini API` · `Vite` · `Vercel`

---

## 🛠️ Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="175em" src="https://github-readme-stats.vercel.app/api?username=Malhar1912&show_icons=true&theme=midnight-purple&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=c084fc&icon_color=a855f7&text_color=e2e8f0"/>
<img height="175em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Malhar1912&layout=compact&langs_count=6&theme=midnight-purple&hide_border=true&bg_color=0d1117&title_color=c084fc&text_color=e2e8f0"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Malhar1912&theme=midnight-purple&hide_border=true&background=0d1117&dates=9ca3af&ring=7C3AED&fire=C4B5FD&currStreakNum=ffffff&sideNums=ffffff&currStreakLabel=c084fc&sideLabels=c084fc)](https://git.io/streak-stats)

</div>

---

## 🤝 Connect

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-Malhar1912-181717?style=for-the-badge&logo=github)](https://github.com/Malhar1912)
[![Email](https://img.shields.io/badge/Email-malharpangarkar19@gmail.com-9333ea?style=for-the-badge&logo=gmail&logoColor=white)](mailto:malharpangarkar19@gmail.com)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2d1b69,50:1a0a3e,100:000000&height=120&section=footer&animation=fadeIn" width="100%"/>

*"The optimizer that penalizes its own frequency components is not afraid of itself."*

![Profile Views](https://komarev.com/ghpvc/?username=Malhar1912&color=9333ea&style=flat-square&label=profile+views)

</div>
