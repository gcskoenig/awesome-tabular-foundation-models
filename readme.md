<div align="center">

<!-- title -->

<!--lint ignore no-dead-urls-->

# Awesome Tabular Foundation Models [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![lint](https://github.com/gcskoenig/awesome-tabular-foundation-models/actions/workflows/lint.yaml/badge.svg)](https://github.com/gcskoenig/awesome-tabular-foundation-models/actions/workflows/lint.yaml)

<!-- subtitle -->

A curated collection of **research papers** on **tabular foundation models**: models pretrained on large-scale (synthetic) data that generalize to unseen tabular tasks at inference time. 
<!-- image -->

<a href="" target="_blank" rel="noopener noreferrer">
  <img src="" />
</a>
</div>

<!-- TOC -->

## Contents

- [Foundation Models](#foundation-models)
- [Theory](#theory)
- [Prior Design](#prior-design)
- [Interpretability](#interpretability)
- [Fast Inference](#fast-inference)
- [Causal Inference](#causal-inference)
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Software and Libraries](#software-and-libraries)
- [Educational](#educational)

<!-- CONTENT -->

## Foundation Models

- [TabPFN: A transformer that solves small tabular classification problems in a second](https://arxiv.org/abs/2207.01848) - The original TabPFN for small tabular classification via in-context learning.
- [TabForestPFN](https://arxiv.org/abs/2405.13396) - Uses forest-based synthetic data generation for complex decision boundaries.
- [TabDPT: Scaling Tabular Foundation Models](https://arxiv.org/abs/2410.18164) - Combines in-context learning with self-supervised learning and demonstrates scaling laws for tabular foundation models.
- [Accurate predictions on small data with a tabular foundation model (TabPFN v2)](https://www.nature.com/articles/s41586-024-08328-6) - Extends TabPFN to regression, multi-class classification, and larger datasets up to 10,000 samples, published in Nature.
- [TabICL: A Tabular Foundation Model for In-Context Learning on Large Data](https://arxiv.org/abs/2502.05564) - Column-then-row attention architecture for efficient in-context learning, ~10x faster than TabPFN v2 on large datasets.
- [TabFlex](https://arxiv.org/abs/2506.05584) - Employs linear attention to scale tabular in-context learning to millions of samples.
- [ContextTab](https://arxiv.org/abs/2506.10707) - Incorporates semantic awareness and is trained on real-world data rather than purely synthetic priors.
- [Real-TabPFN](https://arxiv.org/abs/2507.03971) - Improves TabPFN through continued pre-training on curated real-world datasets.
- [LimiX](https://arxiv.org/abs/2509.03505) - Models the joint distribution over variables and missingness patterns.
- [Mitra](https://arxiv.org/abs/2510.21204) - Combines curated synthetic priors with fine-tuning strategies.
- [TabPFN-Wide](https://arxiv.org/abs/2510.06162) - Specializes in extreme feature counts exceeding 50,000 columns.
- [TabPFN-2.5: Advancing the State of the Art in Tabular Foundation Models](https://arxiv.org/abs/2511.08667) - Scales to 50,000 samples and 2,000 features; state-of-the-art on the TabArena benchmark.
- [Orion-MSP](https://arxiv.org/abs/2511.02818) - Uses multi-scale sparse attention with memory mechanisms for tabular prediction.
- [Orion-Bix](https://arxiv.org/abs/2512.00181) - Implements bi-axial attention for few-shot tabular learning.
- [TabICL v2: A better, faster, scalable, and open tabular foundation model](https://arxiv.org/abs/2602.11139) - Improves speed and performance over TabICL; adds regression support.

## Theory

- [Transformers Can Do Bayesian Inference](https://arxiv.org/abs/2112.10510) - Introduces Prior-Data Fitted Networks (PFNs), showing that transformers can approximate Bayesian posterior predictive distributions via in-context learning.
- [Statistical Foundations of Prior-Data Fitted Networks](https://arxiv.org/abs/2305.11097) - Provides a theoretical analysis of PFNs, including a frequentist interpretation and conditions under which bias and variance vanish.

<!-- END CONTENT -->

## Prior Design

In addition to the foundation model papers:

- [Improving TabPFN's Synthetic Data Generation by Integrating Causal Structure](https://arxiv.org/abs/2603.10254) - Proposes DAG-aware conditioning to align TabPFN's autoregressive generation with causal structure, reducing spurious correlations.

## Interpretability

- [MotherNet: Fast Training and Inference via Hyper-Network Transformers](https://arxiv.org/abs/2312.08598) - Generates the weights of a compact child neural network in a single forward pass, enabling fast inference without in-context overhead.
- [GAMformer: In-Context Learning for Generalized Additive Models](https://arxiv.org/abs/2410.04560) - Estimates interpretable GAM shape functions in a single forward pass, bridging foundation models and interpretable ML.

## Causal Inference

- [Do-PFN: In-Context Learning for Causal Effect Estimation](https://arxiv.org/abs/2506.06039) - Pre-trains PFNs on synthetic data from diverse causal structures including interventions to estimate causal effects without knowing the causal graph.
- [CausalPFN: Amortized Causal Effect Estimation via In-Context Learning](https://arxiv.org/abs/2506.07918) - Amortizes Bayesian causal inference, mapping observational data directly to treatment effect estimates in a single forward pass.
- [CausalFM: Foundation Models for Causal Inference via Prior-Data Fitted Networks](https://arxiv.org/abs/2506.10914) - A comprehensive framework for PFN-based causal inference covering back-door, front-door, and instrumental variable adjustment.

## Fast Inference

Related to interpretability. Anything else?

## Benchmarks and Evaluation

## Software and Libraries

## Educational

- [nanoTabPFN: A Lightweight and Educational Reimplementation of TabPFN](https://arxiv.org/abs/2511.03634) - Under 500 lines of code; achieves competitive performance within one minute of pre-training on a single GPU.
- [NanoTabICL](https://github.com/soda-inria/nanotabicl) - Minimal and educational reimplementation of the TabICLv2 architecture.




## Contributing

[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors

[Thanks goes to these contributors](https://github.com/gcskoenig/awesome-tabular-foundation-models/graphs/contributors)!


## Related Lists


- [awesome-tabpfn](https://github.com/PriorLabs/awesome-tabpfn) - List of awesome applications of TabPFN, curated by the Prior Labs team.


