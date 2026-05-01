# A Bible of Scientific Machine Learning

*Dynamical Systems, Operators, and the Frontier of Physics-Aware Deep Learning*

A personal reference manual covering the mathematical foundations, core
techniques, and emerging frontiers of Scientific Machine Learning (SciML)
— from classical dynamical systems theory through to foundation models for
physics circa 2024–2026.

> **A note from the author.**
> I put this document together as a reference for myself to keep up with the
> rapidly evolving field of Scientific ML. It was generated with the help of
> [Perplexity Computer](https://perplexity.ai/) and Claude Opus, then lightly
> curated for structure and accuracy. **Treat it accordingly:** it is a
> distilled survey rather than a peer-reviewed text. Cross-check any specific
> claim, derivation, or citation against the primary literature before
> relying on it for research or production work. Pull requests with
> corrections are very welcome.

## Why this exists

SciML moves fast — new neural-operator architectures, foundation models for
physics, and generative PDE solvers appear monthly. This document tries to
provide:

- A unified vocabulary that bridges classical numerical analysis, dynamical
  systems theory, and modern deep learning.
- Concise, equation-level summaries of the major method families (PINNs,
  neural operators, Koopman/SINDy, UDEs, equivariant networks,
  diffusion-based simulators, UQ).
- Color-coded **Recipe / Insight / Pitfall** boxes for fast scanning during
  research or paper-writing.
- Pointers into the primary literature for everything covered.

It is aimed at graduate students and researchers already comfortable with
ODE/PDE theory and the basics of deep learning.

## What's inside

- **Part I — Foundations.** Dynamical systems, stability, Hamiltonian /
  Lagrangian mechanics, classical numerical methods (RK, symplectic,
  spectral, FE/FV), adjoints, reduced-order models.
- **Part II — Core SciML toolkit.** Neural ODEs / CDEs / SDEs, PINNs and
  their failure modes, neural operators (DeepONet, FNO, SFNO, GNO,
  Transolver, Poseidon), Koopman / DMD / SINDy, symbolic regression,
  Universal Differential Equations, NeuralGCM, KANs.
- **Part III — Geometry, generative, probabilistic.** $E(3)$/$SE(3)$
  equivariant networks, NequIP / MACE, MeshGraphNets, score-based diffusion
  for PDEs, flow matching and stochastic interpolants, full UQ stack
  (Bayesian DL, ensembles, GPs, conformal prediction).
- **Part IV — Frontier (2024–2026).** Foundation models for physics
  (Poseidon, MPP, DPOT, Aurora, NeuralGCM, GenCast), software ecosystems
  (SciML.jl, JAX, Modulus), benchmarks (PDEBench, The Well, WeatherBench 2,
  CAMELS), emerging trends.
- **Appendices.** Automatic differentiation, functional analysis,
  stochastic calculus, reading list, glossary, method-taxonomy diagram.

The compiled PDF is roughly 55 pages.

## Getting the PDF

The latest build is committed as [`main.pdf`](./main.pdf).

## Building from source

Requires a TeX Live distribution with `latexmk`, `biber`, and the
`tcolorbox`, `fncychap`, `biblatex`, and `tikz` packages.

```bash
latexmk -pdf main.tex
```

To clean intermediate files:

```bash
latexmk -C
```

## Repository layout

```
.
├── main.tex             # master file (preamble + \input chapters)
├── references.bib       # BibTeX entries
├── main.pdf             # latest compiled build
└── chapters/
    ├── preface.tex
    ├── 01_foundations.tex
    ├── 02_classical_numerics.tex
    ├── 03_neural_odes.tex
    ├── 04_pinns.tex
    ├── 05_neural_operators.tex
    ├── 06_operator_theoretic.tex
    ├── 07_hybrid_ude.tex
    ├── 08_geometric_equivariant.tex
    ├── 09_generative_pdes.tex
    ├── 10_uq.tex
    ├── 11_multiscale.tex
    ├── 12_software_benchmarks.tex
    ├── 13_emerging_trends.tex
    └── 14_appendix.tex
```

## Contributing

Spotted an error, an outdated benchmark, or a missing reference? Open an
issue or PR. Each chapter lives in its own file, so contributions can be
scoped tightly.

## Citation

If this reference is useful in your work, you can cite it informally as:

> J. Cunha, *A Bible of Scientific Machine Learning*, GitHub repository,
> 2026. https://github.com/julian-8897/scientific-ml-bible

## License

Released under the [MIT License](./LICENSE) — fork, extend, and adapt
freely.
