## LearningToOptimize Organization

**LearningToOptimize (L2O)** is a collection of open-source tools focusing on the emerging paradigm of amortized optimization - using machine learning methods to speed up traditional constrained optimization solvers. *L2O is a work-in-progress; existing functionality is considered experimental and is subject to change*.

## Open-Source Repositories


|  |  |
|------|-------------------|
| [LearningToOptimize.jl](https://github.com/LearningToOptimize/LearningToOptimize.jl) | Flagship Julia package that wraps data generation, training loops and evaluation utilities for fitting surrogate models to parametric optimization problems. |
| [DecisionRules.jl](https://github.com/andrewrosemberg/DecisionRules.jl) | A package for building decision rules in Multistage Stochastic Problems, as proposed in [*Efficiently Training Deep-Learning Parametric policies using Lagrangian Duality*](https://arxiv.org/pdf/2405.14973). |
| [L2OALM.jl](https://github.com/LearningToOptimize/L2OALM.jl) | Implementation of the primal-dual learning method **ALM**, as proposed in  *[Self-Supervised Primal-Dual Learning for Constrained Optimization](https://ojs.aaai.org/index.php/AAAI/article/view/25520)*. | 
| [L2ODLL.jl](https://github.com/LearningToOptimize/L2ODLL.jl) | Implementation of the dual learning method **DLL**, as proposed in  *[Dual Lagrangian Learning for Conic Optimization](https://neurips.cc/virtual/2024/poster/94146)*.  |
| [L2ODC3.jl](https://github.com/LearningToOptimize/L2ODC3.jl) | Implementation of the primal learning method **DC3**, as proposed in [*DC3: A learning method for optimization with hard constraints*](https://openreview.net/forum?id=V1ZHVxJ6dSS).   |
| [BatchNLPKernels.jl](https://github.com/LearningToOptimize/BatchNLPKernels.jl) | GPU kernels that evaluate objectives, Jacobians and Hessians for **batches** of [ExaModels](https://github.com/exanauts/ExaModels.jl), useful when defining loss functions for batches of ML predictions. |
| [BatchConeKernels.jl](https://github.com/LearningToOptimize/BatchConeKernels.jl) | GPU kernels for batched cone operations (projections, distances, etc.), useful for implementing advanced architectures such as repair layers. |
| [LearningToControlClass](https://github.com/LearningToOptimize/LearningToControlClass) | Course repository for *Special Topics on Optimal Control & Learning* (Fall 2025 at Georgia Tech)|


## Open Datasets and Weights

The [LearningToOptimize 🤗 HuggingFace organization](https://huggingface.co/LearningToOptimize) hosts datasets and pre-trained weights which can be used with L2O packages.

<!--
## Contributing

Issues and pull requests are welcome! Please open an issue first if you plan a large contribution. For questions or collaboration ideas, reach out via the Discussions tab or the Hugging Face community page. We follow the standard [Contributor Covenant code of conduct](https://www.contributor-covenant.org/version/3/0/code_of_conduct/).

-->