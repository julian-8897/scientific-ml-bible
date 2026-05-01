# A Bible of Scientific Machine Learning

*Dynamical Systems, Operators, and the Frontier of Physics-Aware Deep Learning*

A comprehensive reference manual covering classical dynamics, PINNs, neural
operators, Koopman/SINDy methods, equivariant networks, generative
surrogates, uncertainty quantification, and 2024–2026 frontiers.

## Contents

- **Part I — Foundations**: dynamical systems, stability, Hamiltonian/Lagrangian mechanics, classical numerical methods.
- **Part II — Core SciML toolkit**: Neural ODEs/CDEs/SDEs, PINNs, neural operators (DeepONet, FNO, SFNO, GNO, Transolver, Poseidon), Koopman/DMD/SINDy, symbolic regression, UDEs, NeuralGCM, KANs.
- **Part III — Geometry, generative, probabilistic**: $E(3)$/$SE(3)$ equivariant networks, score-based diffusion, flow matching, full UQ stack (BNNs, ensembles, GPs, conformal).
- **Part IV — Frontier**: foundation models for physics, software ecosystems, benchmarks, emerging trends.
- **Appendices**: AD, functional analysis, stochastic calculus, reading list, glossary, method-taxonomy diagram.

## Building

Requires a TeX Live distribution with `latexmk`, `biber`, and the
`tcolorbox`, `fncychap`, `biblatex`, and `tikz` packages.

```bash
latexmk -pdf main.tex
```

The compiled PDF is `main.pdf` (~55 pages).

## Layout

```
.
├── main.tex             # master file
├── references.bib       # BibTeX entries
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

## License

MIT — feel free to fork, extend, and adapt.
