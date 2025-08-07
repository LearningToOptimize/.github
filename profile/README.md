## 🚀 Overview

LearningToOptimize (L2O) is a work-in-progress organization that brings together researchers and practitioners who teach machines to solve optimization problems, rather than hand-coding solvers. We maintain fast Julia libraries, GPU kernels, and course material that make it easy to train optimization proxies (a.k.a. amortized or learned optimizers) and prove they satisfy real-world constraints.  ￼

----

## 📚 Repository catalogue

(In order of maturity)

| Repo | Objective / scope |
|------|-------------------|
| [LearningToOptimize.jl](https://github.com/LearningToOptimize/LearningToOptimize.jl) | Flagship Julia package that wraps data generation, training loops and evaluation utilities for fitting surrogate models to parametric optimization problems. |
| [BatchNLPKernels.jl](https://github.com/LearningToOptimize/BatchNLPKernels.jl) | CUDA kernels (via `KernelAbstractions.jl`) that evaluate objectives, Jacobians and Hessians for **batches** of `ExaModel`s, enabling large-scale differentiable nonlinear programming on GPUs. |
| [L2OALM.jl](https://github.com/LearningToOptimize/L2OALM.jl) | Implementation of *Learning-to-Optimize via Augmented-Lagrangian Primal–Dual* (ALM): learns fast proxies while enforcing equality / inequality constraints through a differentiable ALM inner loop. | 
| [L2ODLL.jl](https://github.com/LearningToOptimize/L2ODLL.jl) | Implements *Dual Lagrangian Learning* (DLL) for conic programs; couples a neural proxy with dual variables to guarantee feasibility and tight optimality gaps.  |
| [L2ODC3.jl](https://github.com/LearningToOptimize/L2ODC3.jl) | Prototype of **DC3 – Deep Constraint Completion & Correction**: a differentiable pipeline that completes outputs to satisfy equalities and iteratively corrects inequalities, offering hard-constraint guarantees for learned optimizers.   |
| [BatchConeKernels.jl](https://github.com/LearningToOptimize/BatchConeKernels.jl) | Companion GPU kernels that accelerate batched cone operations (SOC, PSD, etc.)—useful for conic optimizers and neural-network constraint layers. *(public README not yet available)* |
| [DecisionRules.jl](https://github.com/andrewrosemberg/DecisionRules.jl) | Tools to build and train decision-rule policies for multistage stochastic programs, following the two-stage ML-guided framework in recent research. |

### Course

| Repo | Objective / scope |
|------|-------------------|
| [LearningToControlClass](https://github.com/LearningToOptimize/LearningToControlClass) | Complete materials for the graduate seminar *Special Topics on Optimal Control & Learning* (Fall 2025 — Georgia Tech): lecture notes, slides, homework, and project templates. |

----

## 🤗 Hugging Face resources

Looking for datasets, pretrained proxies, or benchmarking notebooks? Check the companion Hugging Face org LearningToOptimize. There you’ll find curated parametric-optimization datasets, ready-to-use model checkpoints, and tutorials that complement the Julia libraries above.  ￼

----

## 🔗 Getting started

# Add the main package

```julia
julia> ] add LearningToOptimize
# Or clone a specialized kernel repo
git clone https://github.com/LearningToOptimize/BatchNLPKernels.jl
```

Refer to each repository’s README for installation specifics and API docs.

----

## 🤝 Contributing

Issues and pull requests are welcome! Please open an issue first if you plan a large contribution. For questions or collaboration ideas, reach out via the Discussions tab or the Hugging Face community page. We follow the standard Contributor Covenant code of conduct.

----

Happy optimizing!
