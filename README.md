# Swarm Intelligence Lab

An academic and educational repository for the **study, implementation, and visualization** of *Swarm Intelligence* algorithms, following as a reference the paper:

> **Swarm Intelligence: A Review of Algorithms**  
> Amrita Chakraborty, Arpan Kumar Kar (2017)

The goal of this project is to **learn how swarm intelligence algorithms work**, implement them **from scratch**, and analyze their behavior through **reproducible experiments and visualizations**.

---

## Project Goals

- Study swarm intelligence algorithms **organized by biological inspiration**
- Implement each algorithm incrementally and in a documented manner
- Compare their behavior on classical benchmark problems
- Visualize their dynamics (exploration, exploitation, convergence)
- Serve as an **educational reference**, not as an official benchmark

---

## Algorithms Included (as reviewed in the paper)

### 🐜 Insect-based
- Ant Colony Optimization (ACO)
- Artificial Bee Colony (ABC)
- Firefly Algorithm (FA)
- Glowworm Swarm Optimization (GSO)

### 🐾 Animal-based
- Bat Algorithm (BA)
- Grey Wolf Optimizer (GWO)
- Lion Optimization Algorithm (LOA)
- Spider Monkey Optimization (SMO)

> ⚠️ This repository intentionally **does not include algorithms outside the paper**
> (e.g. PSO), in order to keep the scope academically consistent.

---

## Project Structure

```
src/si/
├── algorithms/        # Implementations (organized by family)
│   ├── insect/
│   │   ├── ant/aco.py
│   │   ├── bee/abc.py
│   │   ├── firefly/fa.py
│   │   └── glowworm/gso.py
│   ├── animal/
│   │   ├── bat/ba.py
│   │   ├── wolf/gwo.py
│   │   ├── lion/loa.py
│   │   └── spider_monkey/smo.py
│   └── baseline/
│       └── random_search.py
│
├── benchmarks/        # Benchmark functions and problems
├── viz/               # Visualization utilities (matplotlib)
├── experiments/       # Experiment runner and orchestration
├── utils/             # Shared utilities
└── interfaces/        # Common types and contracts
```

---

## Visualization (Academic Focus)

Visualizations are implemented using **Matplotlib**, which is the standard tool in academic environments.

Depending on the algorithm type, the following visualizations are planned:

- **Continuous 2D optimization**
  - contour / heatmap plots
  - agent positions per iteration
  - convergence curves

- **Discrete problems (ACO)**
  - routes (e.g. TSP)
  - evolution of the best tour

The goal of visualization is **to understand algorithm behavior**, not only final performance.

---

## Testing Philosophy

Tests in this project focus on correctness and learning rather than formal proofs:

- Benchmark functions correctness
- Algorithm interface consistency
- Basic reproducibility using fixed random seeds
- Smoke tests to catch implementation errors early

This approach allows safe experimentation while learning.

---

## Installation

Requires **Python 3.10+**.

```bash
pip install -e .
```

Main dependencies:
- numpy
- matplotlib
- pyyaml
- pytest

---

## Project Status

🚧 **Work in progress**

- Repository structure is defined
- Algorithms are implemented incrementally
- Visualizations are added as implementations mature

---

## Academic Disclaimer

This project:
- ❌ does not replicate exact results from the paper
- ❌ is not intended as an official benchmark
- ✅ is educational and exploratory
- ✅ prioritizes clarity and understanding over performance claims

---

## License

MIT (can be changed if needed).

