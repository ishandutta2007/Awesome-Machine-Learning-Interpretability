# Awesome-Machine-Learning-Interpretability

## Top Machine Learning Interpretability Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Model Explanation, Fairness Auditing & Self-Hosted Interpretability Toolkits*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Machine Learning Interpretability**. These tools help teams understand and trust model behavior—explaining individual predictions, surfacing global feature importance, auditing for bias, and monitoring for drift—so stakeholders can act on model outputs with confidence and regulators can verify compliance.



**Examples** include InterpretML, SHAP, LIME, Fiddler AI, Arize AI, Arthur AI, and TruLens (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding per-inference SaaS fees, and controlling the explanation layer. The open-source landscape is anchored by **InterpretML** (Microsoft's unified glassbox/blackbox toolkit with the Explainable Boosting Machine), **SHAP** (the game-theoretic attribution standard), and **LIME** (the original local surrogate method), with **TruLens** serving LLM/RAG evaluation and **Captum** providing PyTorch-native explanations.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



| Product | Description | Pricing | Free Tier Limit |

| :--- | :--- | :--- | :--- |

| **[Arize AI](https://arize.com/)** | AI observability platform with explainability for tabular and LLM models. | **AX Pro**: **$50/month** . **AX Enterprise**: custom, with self-hosted deployment option . | **AX Free**: 25k spans/month, 1 GB storage, 15-day retention, unlimited users, unlimited evaluations . |

| **[Arthur AI](https://www.arthur.ai/)** | AI governance platform with explainability, fairness, and "What-If" analysis. | **Premium**: **$60/month** . **Enterprise**: custom (VPC, SSO, SLAs) . | **Free**: 4 use cases, 1 org, 1 workspace, 300k spans, 12k inferences, 7-day retention, unlimited seats . |

| **[Fiddler AI](https://www.fiddler.ai/)** | Model performance monitoring and explainable AI platform with decoupled pricing for monitoring, explainability, and fairness. | Usage-based with annual commitment. Metrics: data ingested, models, explanations, retention months. **Lite** and **Standard** plans; contact sales for estimate . | No permanent free tier. **Pricing estimate available** via sales request . |

| **[TruEra (Snowflake)](https://www.truera.com/)** | AI observability and explainability platform. **Acquired by Snowflake (May 2024)**. | **TruLens (open-source)**: free under Apache 2.0. **Commercial**: now billed via Snowflake credits as part of Cortex/AI Observability . | **TruLens**: fully free and open-source. **Legacy TruEra**: no standalone free tier; access via Snowflake trial credits. |

| **[WhyLabs](https://whylabs.ai/)** | AI observability platform. **Transitioned to fully open-source** (Apache 2.0) after Apple acquisition (2025). | **Open Source**: Free (entire platform including whylogs and langkit). Legacy SaaS tiers on AWS Marketplace: $100/mo (2 models), $200/mo (3 models), Enterprise $8,333/mo . | **Entire platform is now free and open-source**. Legacy "1 Model" tier remains on marketplace . |

| **[H2O.ai](https://h2o.ai/)** | Enterprise AI platform with Driverless AI (AutoML) including built-in interpretability (variable importance, reason codes). | **H2O-3**: free (Apache 2.0). **Driverless AI**: enterprise licensing, typically **from $10,000/year** . | **H2O-3**: fully free. **Driverless AI**: free trial available; no permanent free tier . |

| **[DataRobot](https://www.datarobot.com/)** | Automated ML platform with prediction explanations and model interpretation built into deployments. | **Pricing 5.0 (Classic MLOps)**: contact sales; no public list prices . | No public free tier. Trial available via sales engagement. |

| **[Dataiku](https://www.dataiku.com/)** | Collaborative data science platform with visual and code-based workflows, including model interpretability features. | **Highly customized**, typically **$150K–$300K+ for 25 users/year** for enterprise deployment . | **14-day Cloud Trial**: 5 users, all features except Govern/advanced LLM Mesh. **Free Edition** for on-prem (feature-restricted). |

| **[Alteryx](https://www.alteryx.com/)** | Data analytics platform with predictive tools including interpretability features. | Designer licenses **~$5,195+/user/year**; **25 users, 1 year: $100K–$150K** . | **30-day free trial**. No permanent free tier. |

| **[IBM Watson OpenScale](https://www.ibm.com/products/watson-openscale)** | AI governance and explainability platform for monitoring model fairness and drift. | Contact vendor for pricing; Capterra lists a **$49 flat rate** (likely legacy/limited offering) . | No public free tier details available. |



## Open-Source GitHub Projects



- **[InterpretML](https://github.com/interpretml/interpret)** [![GitHub Stars](https://img.shields.io/github/stars/interpretml/interpret?style=social&color=white)](https://github.com/interpretml/interpret/stargazers)  

  **Microsoft's unified glassbox and blackbox toolkit.** Provides **Explainable Boosting Machine (EBM)**—a glassbox model competitive with gradient boosting while being fully interpretable—plus SHAP, LIME, and partial dependence plots in one API. **Strengths**: one interface for both inherently interpretable models and post-hoc explanations. Best for teams wanting to choose between transparent models and blackbox explanations without leaving one library.



- **[SHAP](https://github.com/slundberg/shap)** [![GitHub Stars](https://img.shields.io/github/stars/slundberg/shap?style=social&color=white)](https://github.com/slundberg/shap/stargazers)  

  **The game-theoretic attribution standard.** Implements Shapley values to assign each feature a contribution to the prediction—theoretically grounded and consistent. **Model-agnostic** with optimized implementations for tree models (XGBoost, LightGBM). **Visualizations**: force plots, summary plots, dependence plots, waterfall charts. Best for teams wanting the most widely accepted, defensible feature attribution method.



- **[LIME](https://github.com/marcotcr/lime)** [![GitHub Stars](https://img.shields.io/github/stars/marcotcr/lime?style=social&color=white)](https://github.com/marcotcr/lime/stargazers)  

  **The original local surrogate method.** Explains individual predictions by fitting a simple interpretable model to perturbations around the prediction point. **Model-agnostic** and conceptually intuitive. **Limitations**: sampling-based and can be unstable across runs. Best for quick, intuitive local explanations and as a complement to SHAP's global consistency.



- **[TruLens](https://github.com/truera/trulens)** [![GitHub Stars](https://img.shields.io/github/stars/truera/trulens?style=social&color=white)](https://github.com/truera/trulens/stargazers)  

  **The LLM and RAG evaluation standard.** Free under Apache 2.0. Provides feedback functions, tracing, and evaluation for LLM applications—including groundedness, relevance, and context adherence. **Note**: TruLens is now the primary open-source offering from the TruEra team post-Snowflake acquisition . Best for teams building LLM applications that need to evaluate and explain retrieval-augmented generation pipelines.



- **[Captum](https://github.com/pytorch/captum)** [![GitHub Stars](https://img.shields.io/github/stars/pytorch/captum?style=social&color=white)](https://github.com/pytorch/captum/stargazers)  

  **The PyTorch-native interpretation library.** Implements integrated gradients, saliency maps, GradCAM, DeepLIFT, and Shapley values specifically for PyTorch models. **Strengths**: tight integration with PyTorch autograd; optimized for deep learning workflows. Best for PyTorch practitioners needing gradient-based explanations for neural networks.



- **[Alibi](https://github.com/SeldonIO/alibi)** [![GitHub Stars](https://img.shields.io/github/stars/SeldonIO/alibi?style=social&color=white)](https://github.com/SeldonIO/alibi/stargazers)  

  **The Seldon-backed explanation library.** Supports TensorFlow and PyTorch with anchor explanations, counterfactuals, integrated gradients, and kernel SHAP. **Strengths**: strong on counterfactual explanations ("what minimal change would flip the prediction?"). Best for teams needing counterfactual analysis alongside standard attribution.



- **[dalex](https://github.com/ModelOriented/DALEX)** [![GitHub Stars](https://img.shields.io/github/stars/ModelOriented/DALEX?style=social&color=white)](https://github.com/ModelOriented/DALEX/stargazers)  

  **The model-agnostic exploration toolkit.** R and Python versions with break-down plots, SHAP, partial dependence, and model performance diagnostics. Best for R users and teams wanting a unified exploration workflow across languages.



### Additional Strong Open-Source Options



- **eli5** — Older but still useful library for debugging ML classifiers and inspecting feature importances. Best for quick sanity checks on scikit-learn models.

- **shapash** — Web-based dashboard for SHAP-based explanations, designed for business stakeholders. Best for teams wanting to share explanations without building a custom UI.

- **LIT (Learning Interpretability Tool)** — Google's interactive UI for exploring model behavior, counterfactuals, and saliency. Best for researchers wanting a visual debugging environment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **SaaS interpretability pricing is often opaque**: Fiddler requires sales engagement for quotes; DataRobot and Dataiku use custom enterprise pricing . Arize and Arthur offer transparent tiers but scale with span volume .

- **WhyLabs and TruEra have fundamentally changed**: WhyLabs is now fully open-source after Apple's acquisition; TruEra's commercial offering is now part of Snowflake . Legacy pricing on marketplaces may not reflect current reality.

- **SHAP and LIME answer different questions**: SHAP provides consistent, game-theoretic attributions; LIME provides local approximations that are intuitive but can be unstable. Many teams use both.

- **Interpretability is not fairness**: SHAP tells you *why* a prediction happened, not whether the model is fair. Pair with dedicated fairness auditing tools for compliance.



---



**Made for data scientists, ML engineers, and organizations building transparent, accountable machine learning systems.**  

Let's make ML interpretability more open, rigorous, and accessible.
