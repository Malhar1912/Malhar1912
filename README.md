<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a0a00,30:3d1a00,60:6b3a1f,100:c8963e&height=240&section=header&text=Malhar%20Pangarkar&fontSize=58&fontColor=f5e6c8&fontAlignY=40&desc=∿%20where%20mathematics%20meets%20something%20that%20feels%20like%20longing%20∿&descAlignY=62&descSize=14&animation=fadeIn&fontAlign=50" width="100%"/>

</div>

<br/>

<div align="center">

<a href="https://github.com/Malhar1912/NATO"><img src="https://img.shields.io/badge/✦%20nato--opt%20on%20PyPI-install%20it-c8963e?style=for-the-badge&labelColor=2a1200&color=c8963e" /></a>
&nbsp;
<a href="mailto:malharpangarkar08@gmail.com"><img src="https://img.shields.io/badge/✦%20reach%20me-malharpangarkar08-c8963e?style=for-the-badge&labelColor=2a1200&color=c8963e" /></a>

</div>

<br/>

<div align="center">

```
          ❝  some people write about love.
               i write about constrained optimization,
                 hyperbolic manifolds,
                   and the things computers
                     can never know.  ❞
```

</div>

---

<br/>

## ✦ &nbsp; a c t &nbsp; i &nbsp; — &nbsp; *published*

<br/>

### &nbsp;&nbsp;&nbsp;**[NATO — Neural Adaptive Training Optimizer](https://github.com/Malhar1912/NATO)**

<div align="center">

> *there are optimizers, and then there are optimizers that filter their own gradients through an FFT.*

</div>

&nbsp;&nbsp;&nbsp;&nbsp;`pip install nato-opt` &nbsp;·&nbsp; co-authored with Atharva Khambete &nbsp;·&nbsp; GPU/CUDA native &nbsp;·&nbsp; MIT

&nbsp;&nbsp;&nbsp;&nbsp;Three original techniques, zero extra forward-pass cost —

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Fourier Spectral Penalty** — regularises weights in the frequency domain, not the weight domain.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**Kakeya Directional Penalty** — penalises gradient directions that are too consistent. force the model to explore.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**N-D FFT Gradient Filtering** — smooths high-frequency gradient noise before every step.

```python
from nato_opt import NATOOptimizer, fourier_spectral_penalty, low_pass_filter_gradients

optimizer  = NATOOptimizer(model.parameters(), lr=1e-3)
fsp        = fourier_spectral_penalty(model, lambda_fsp=1e-6)
low_pass_filter_gradients(model, cutoff_ratio=0.5)
optimizer.step(epoch)
```

[![PyPI](https://img.shields.io/pypi/v/nato-opt?color=c8963e&style=flat-square&logo=pypi&logoColor=f5e6c8&label=nato-opt)](https://pypi.org/project/nato-opt/)
![Python](https://img.shields.io/badge/python-3.8+-8b6914?style=flat-square)
![CUDA](https://img.shields.io/badge/cuda-accelerated-76b900?style=flat-square&logo=nvidia&logoColor=white)

<br/>

---

<br/>

## ✦ &nbsp; a c t &nbsp; i i &nbsp; — &nbsp; *manuscripts*

<br/>

### &nbsp;&nbsp;&nbsp;**[GeoSDE-IDS — Geometric Stochastic Differential Intrusion Detection](https://github.com/Malhar1912/GeoSDE-IDS)**

<div align="center">

> *what if network traffic anomalies are not outliers in Euclidean space —  
> but curvature distortions on a hyperbolic manifold?*

</div>

&nbsp;&nbsp;&nbsp;&nbsp;Full Elsevier manuscript (`paper/elsevier_manuscript.tex`). Three datasets. Five seeds. Reproducibility checklist.

&nbsp;&nbsp;&nbsp;&nbsp;The detection engine runs **five geometric signals** simultaneously —

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;① Ollivier-Ricci Curvature distortion &nbsp;② Dirichlet Energy Functional acceleration  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;③ Möbius Invariance violation &nbsp;④ Fokker-Planck Density evolution (KL-Divergence)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;⑤ SDE Drift Deviation

&nbsp;&nbsp;&nbsp;&nbsp;Fused via meta-classifier (LR + MLP). Benchmarked on CIC-IDS 2017, NSL-KDD, UNSW-NB15.

![Python](https://img.shields.io/badge/python-stochastic%20geometry-8b6914?style=flat-square)
![TeX](https://img.shields.io/badge/LaTeX-manuscript-c8963e?style=flat-square&logo=latex&logoColor=white)
![Datasets](https://img.shields.io/badge/datasets-3%20×%205%20seeds-6b3a1f?style=flat-square)

<br/>

### &nbsp;&nbsp;&nbsp;**[TCR — Threshold-Constrained Replay Framework](https://github.com/Malhar1912/Threshold-Constrained-Replay-TCR-A-Constrained-Multi-Objective-Replay-Framework)**

<div align="center">

> *experience replay, but as a constrained stochastic resource allocation problem.  
> prioritized replay never asked why it was doing the ranking.*

</div>

&nbsp;&nbsp;&nbsp;&nbsp;Seven phases. Formal objectives. Ablation gates. The optimisation problem at its heart:

$$\max_{q \in \Delta}\ \mathbb{E}_{\tau \sim q}[\Delta \mathcal{L}(\tau)] \quad \text{s.t.} \quad \mathrm{KL}(q \| p) \le \varepsilon, \quad |D^*| \le B$$

&nbsp;&nbsp;&nbsp;&nbsp;Phase 0.4 validation must pass (ρ > 0.3, p < 0.05, ≥80% of envs) before Phases 1–7 proceed.  
&nbsp;&nbsp;&nbsp;&nbsp;Benchmarks against PER, DreamerV3 native, Uniform Replay — Atari-100k · DMC · Procgen.

![Python](https://img.shields.io/badge/python-reinforcement%20learning-8b6914?style=flat-square)
![Status](https://img.shields.io/badge/status-in%20progress-c8963e?style=flat-square)

<br/>

---

<br/>

## ✦ &nbsp; a c t &nbsp; i i i &nbsp; — &nbsp; *interactive*

<br/>

<table>
<tr>
<td width="50%" valign="top">

### &nbsp;[SAT Solver](https://github.com/Malhar1912/SAT_Solver)

> *formal methods, made visible.*

DPLL with unit propagation and pure literal elimination — rendered as a live decision tree. Green = satisfiable. Red = contradiction.  
Watch NP-complete problems sweat in real time.

`Python` · `networkx` · `MIT`

</td>
<td width="50%" valign="top">

### &nbsp;[Halting Problem Simulation](https://github.com/Malhar1912/Halting_Problem_Simulation) · [↗](https://halting-problem-simulation.vercel.app)

> *the proof you send when someone asks why we can't just verify everything.*

Cyberpunk React app. Animated REBEL paradox walkthrough. Formal proof. Turing, Church, Gödel citations. AGI implications. Deployed.

`TypeScript` · `Framer Motion` · `Vercel`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### &nbsp;[Q-Shield](https://github.com/Malhar1912/Q-Shield-Quaternionic-Key-Exchange-Explorer) · [↗](https://q-shield-quaternionic-key-exchange.vercel.app)

> *key exchange over ℍ, because elliptic curves felt too comfortable.*

Interactive post-quantum cryptography explorer built on quaternion algebra. TypeScript, deployed to production.

`TypeScript` · `Abstract Algebra` · `Vercel`

</td>
<td width="50%" valign="top">

### &nbsp;[LT-Graph](https://github.com/Malhar1912/LT-Graph) · [↗](https://lt-graph.vercel.app)

> *graph theory with a simulation layer and a Gemini-powered brain.*

Interactive traversal toolkit. Components, services, simulation, tests — all there. Deployed.

`TypeScript` · `Gemini API` · `Vite`

</td>
</tr>
</table>

<br/>

---

<br/>

## ✦ &nbsp; s t a c k

<div align="center">

![Python](https://img.shields.io/badge/Python-2a1200?style=for-the-badge&logo=python&logoColor=c8963e)
![TypeScript](https://img.shields.io/badge/TypeScript-2a1200?style=for-the-badge&logo=typescript&logoColor=c8963e)
![PyTorch](https://img.shields.io/badge/PyTorch-2a1200?style=for-the-badge&logo=pytorch&logoColor=c8963e)
![React](https://img.shields.io/badge/React-2a1200?style=for-the-badge&logo=react&logoColor=c8963e)
![C++](https://img.shields.io/badge/C++-2a1200?style=for-the-badge&logo=cplusplus&logoColor=c8963e)
![Rust](https://img.shields.io/badge/Rust-2a1200?style=for-the-badge&logo=rust&logoColor=c8963e)
![LaTeX](https://img.shields.io/badge/LaTeX-2a1200?style=for-the-badge&logo=latex&logoColor=c8963e)
![CUDA](https://img.shields.io/badge/CUDA-2a1200?style=for-the-badge&logo=nvidia&logoColor=c8963e)

</div>

<br/>

---

<br/>

## ✦ &nbsp; s t a t s

<div align="center">

<img height="172em" src="https://github-readme-stats.vercel.app/api?username=Malhar1912&show_icons=true&hide_border=true&bg_color=120800&title_color=c8963e&icon_color=8b6914&text_color=f5e6c8&include_all_commits=true&count_private=true"/>
<img height="172em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Malhar1912&layout=compact&langs_count=7&hide_border=true&bg_color=120800&title_color=c8963e&text_color=f5e6c8&hide=html,css"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=Malhar1912&hide_border=true&background=120800&dates=8b6914&ring=c8963e&fire=f5e6c8&currStreakNum=f5e6c8&sideNums=f5e6c8&currStreakLabel=c8963e&sideLabels=c8963e)](https://git.io/streak-stats)

</div>

<br/>

---

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:c8963e,40:6b3a1f,70:3d1a00,100:1a0a00&height=130&section=footer&animation=fadeIn" width="100%"/>

<br/>

*∿ &nbsp; build something that shouldn't exist yet &nbsp; ∿*

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=Malhar1912&color=c8963e&style=flat-square&label=visitors)

</div>
