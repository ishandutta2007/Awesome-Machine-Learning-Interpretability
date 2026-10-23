<div align="center">

<p align="center">
  <img src="./assets/banner.svg" alt="Awesome Machine Learning Interpretability Banner" width="100%">
</p>

# 🔍 Awesome Machine Learning Interpretability (XAI) 🌟

[![Awesome](https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github)](https://github.com/ishandutta2007/Awesome-Awesome-Awesome)<a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
[![GitHub_Stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-Machine-Learning-Interpretability?style=social&color=white)](https://github.com/ishandutta2007/Awesome-Machine-Learning-Interpretability/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/ishandutta2007/Awesome-Machine-Learning-Interpretability?style=social&color=white)](https://github.com/ishandutta2007/Awesome-Machine-Learning-Interpretability/network/members)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/ishandutta2007/Awesome-Machine-Learning-Interpretability/pulls)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

<p align="center">
  <strong>Curated ecosystem of SaaS platforms, frameworks, and open-source tools for Explainable AI (XAI), Model Auditing, Glassbox Modeling, and Fairness Evaluation.</strong>
</p>

<p align="center">
  <em>Last updated: October 2026 &bull; Maintained by <a href="https://github.com/ishandutta2007">Ishan Dutta</a></em>
</p>

</div>

---

## 📌 Table of Contents

- [📖 Introduction](#-introduction)
- [📊 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS/Hosted Platforms](#️-saashosted-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [⭐ Star History](#-star-history)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [⚖️ Disclaimer](#️-disclaimer)

---

## 📖 Introduction

Machine Learning Interpretability (often categorized under **Explainable AI** or **XAI**) has transitioned from an academic research endeavor to an essential enterprise requirement. As AI regulations tighten (such as the EU AI Act) and foundation models deploy into mission-critical healthcare, financial services, and legal workflows, organizations require mathematical transparency, feature attribution, counterfactual reasoning, and rigorous bias audits.

This guide tracks leading **SaaS platforms** and self-hosted **open-source libraries** that allow data scientists and ML engineers to unpack black-box models, quantify feature importances, detect data drift, and ensure algorithmic fairness.

---

## 📊 Sector Overview & Market Dynamics

The global **AI Governance, Explainability, and Model Observability** market is estimated at **$1.8B to $2.4B in 2026**, on pace to expand past **$6.5B by 2030** at a Compound Annual Growth Rate (CAGR) of over **35%**. 

From a competitive standpoint, the sector remains **moderately fragmented**:
- **Consolidation by Cloud & Data Platforms**: Broad data clouds (Snowflake acquiring TruEra, Apple acquiring WhyLabs, Dynatrace acquiring Arize AI) and hyperscalers (IBM watsonx, AWS SageMaker) are rapidly rolling governance and evaluation tooling into primary platforms.
- **Durable Open-Source Foundation**: Unlike consumer tech, core algorithmic interpretability is not "winner-take-all"—it is anchored by foundational open-source standards like **SHAP** and **InterpretML/EBM**, while specialized startups compete aggressively on real-time LLM tracing, guardrails, and compliance dashboards.

---

## ☁️ SaaS/Hosted Platforms

The following enterprise platforms provide managed dashboards, scalable compute backends, compliance reporting, and real-time inference monitoring.

| Product | Description | Company Scale / Valuation / Revenue | Pricing | Free Tier Limit |
| :--- | :--- | :--- | :--- | :--- |
| **[IBM Watson OpenScale](https://www.ibm.com/products/watson-openscale)** | AI governance and explainability platform for monitoring model fairness, drift, and explanations. | **~$235B Market Cap** (~$67.5B FY revenue) | **Essentials tier**: **$0.60 per Resource Unit (RU)** on IBM Cloud; **Risk & Compliance**: from **$3,500/month** | **Lite Plan (Free forever)**: 1 instance, up to 50,000 transaction rows for debiasing/evaluations, internal managed DB |
| **[TruEra (Snowflake)](https://www.truera.com/)** | AI observability and explainability platform. Acquired by Snowflake (May 2024); integrated into Snowflake Cortex. | **~$115B Market Cap** (Snowflake parent; ~$4.7B+ revenue) | **Snowflake Cortex / Observability**: billed via Snowflake credits; Standard edition starts at **~$2.00–$3.00/credit**; TruLens open-source is **$0** (Apache 2.0) | **30-day free trial**: includes **$400 in usage credits** for virtual warehouses and cloud storage (no permanent free tier for hosted platform) |
| **[DataRobot](https://www.datarobot.com/)** | Automated ML platform with prediction explanations and model interpretation built into deployments. | **$6.3B Valuation** (~$250M+ ARR) | Entry-level commercial contracts start from **~$50,000/year** (custom quote-based on modeling workers and prediction volume) | **30-day SaaS trial**: shared modeling workers, capped at 1,000 LLM calls, 15 vector DBs, batch predictions only (no GPU/NIM) |
| **[Alteryx](https://www.alteryx.com/)** | Data analytics and ML platform with interactive predictive tools and model explainability features. | **$4.4B Valuation** (Acquired/Private; ~$970M revenue) | **Designer Desktop**: starts at **$5,195/user/year**; enterprise team bundles typically start around **$100,000/year** (25 users) | **30-day free trial**: 1 trial workspace, up to 10 invited team members, full Enterprise Designer feature set (expires after 30 days) |
| **[Dataiku](https://www.dataiku.com/)** | Collaborative data science and AI platform with AutoML, model diagnostics, and visual model interpretability. | **$3.7B Valuation** (~$350M+ ARR) | Enterprise tiers typically range from **$150,000–$300,000/year** for 25 users; **Discover Cloud tier**: starting around **$1,500/month** | **Free Edition (Self-hosted, free forever)**: up to 3 users, full Visual ML/AutoML and local compute (excludes automated API/batch deployment nodes). **Cloud Trial**: 14 days, up to 5 users |
| **[H2O.ai](https://h2o.ai/)** | Enterprise AI platform with Driverless AI providing automatic interpretability (variable importance, Shapley values, reason codes). | **$1.7B Valuation** (~$75M ARR) | **Driverless AI**: enterprise licensing starting from **$10,000/year**; **H2O-3** is **$0** (free, Apache 2.0) | **21-day free trial**: full Driverless AI license key in cloud or on-prem. Also offers a 2-hour instant test drive on Aquarium Cloud |
| **[Arize AI](https://arize.com/)** | AI observability platform with explainability for tabular models and LLM applications. | **$915M Valuation** (Acquired by Dynatrace, Aug 2026; ~$45M ARR) | **AX Pro**: **$50/month**; **AX Enterprise**: custom quote with self-hosted / VPC deployment option | **AX Free (Free forever)**: 25k spans/month, 1 GB storage, 15-day data retention, unlimited users, unlimited evaluations |
| **[Fiddler AI](https://www.fiddler.ai/)** | Model performance monitoring and explainable AI platform with decoupled pricing for monitoring, explainability, and fairness. | **~$100M Funding** (Venture-backed Series C) | **Lite Tier (AWS Marketplace)**: starts from **~$2,000/month** ($24,000/year) for 1 model and 0.5 GB/month; custom enterprise quotes for scaled workloads | **30-day free trial**: up to 5 models via AWS SageMaker Partner AI Apps integration; 14-day trial for standalone Guardrails API |
| **[WhyLabs](https://whylabs.ai/)** | AI observability and data drift tracking platform. Transitioned to open source post-Apple acquisition. | **~$37M Valuation** (Acquired by Apple, 2025; raised $14M total) | **Open Source**: **$0** (entire platform including whylogs and langkit); Legacy AWS Marketplace tiers start at **$100/month** (2 models) | **Free forever**: core platform is 100% free and open-source under Apache 2.0. Legacy SaaS tier offers 1 free model on marketplace |
| **[Arthur AI](https://www.arthur.ai/)** | AI governance platform with explainability, fairness auditing, and "What-If" analysis. | **~$30M–$50M Valuation** (Raised ~$60M total venture funding) | **Premium**: **$60/month**; **Enterprise**: custom quote (dedicated VPC, custom SLAs, SSO) | **Free Tier (Free forever)**: 4 use cases, 1 organization, 1 workspace, 300k spans, 12k inferences, 7-day retention, unlimited seats |

---

## 💻 Open-Source GitHub Projects

Sorted by GitHub_Stars (descending) 🌟 to highlight industry adoption and community vitality.

1. **[SHAP (SHapley Additive exPlanations)](https://github.com/slundberg/shap)** [![GitHub_Stars](https://img.shields.io/github/stars/slundberg/shap?style=social&color=white)](https://github.com/slundberg/shap/stargazers)  
   **The game-theoretic attribution standard.** Connects optimal credit allocation with local explanations using Shapley values. Fast TreeSHAP implementation accelerates calculations for XGBoost, LightGBM, and CatBoost. Best for theoretical consistency and production-grade tabular attribution.

2. **[PyTorch Grad-CAM](https://github.com/jacobgil/pytorch-grad-cam)** [![GitHub_Stars](https://img.shields.io/github/stars/jacobgil/pytorch-grad-cam?style=social&color=white)](https://github.com/jacobgil/pytorch-grad-cam/stargazers)  
   **Visual AI explanations and saliency maps for PyTorch.** State-of-the-art implementations of GradCAM, GradCAM++, Score-CAM, Eigen-CAM, and LayerCAM across classification, object detection, and semantic segmentation vision architectures.

3. **[LIME (Local Interpretable Model-agnostic Explanations)](https://github.com/marcotcr/lime)** [![GitHub_Stars](https://img.shields.io/github/stars/marcotcr/lime?style=social&color=white)](https://github.com/marcotcr/lime/stargazers)  
   **The original surrogate explanation engine.** Perturbs input instances to fit sparse, interpretable linear models locally around specific predictions. Best for quick black-box sanity checks across tabular, text, and image domains.

4. **[Evidently AI](https://github.com/evidentlyai/evidently)** [![GitHub_Stars](https://img.shields.io/github/stars/evidentlyai/evidently?style=social&color=white)](https://github.com/evidentlyai/evidently/stargazers)  
   **Evaluation and observability for tabular & LLM systems.** Generates interactive visual reports and JSON test suites to detect data drift, concept drift, feature distribution changes, and regression/classification model degradation.

5. **[InterpretML](https://github.com/interpretml/interpret)** [![GitHub_Stars](https://img.shields.io/github/stars/interpretml/interpret?style=social&color=white)](https://github.com/interpretml/interpret/stargazers)  
   **Microsoft's glassbox and blackbox unified framework.** Houses the **Explainable Boosting Machine (EBM)**—an exact Generalized Additive Model with pairwise interactions (GA²M) that matches the accuracy of Random Forests or GBDTs while preserving 100% global and local interpretability.

6. **[Captum](https://github.com/pytorch/captum)** [![GitHub_Stars](https://img.shields.io/github/stars/pytorch/captum?style=social&color=white)](https://github.com/pytorch/captum/stargazers)  
   **PyTorch official model interpretability library.** Provides native, autograd-integrated implementations of Integrated Gradients, DeepLIFT, Guided Backprop, Saliency, Noise Tunnel, and Shapley Value Sampling for complex deep neural networks.

7. **[Lucid](https://github.com/tensorflow/lucid)** [![GitHub_Stars](https://img.shields.io/github/stars/tensorflow/lucid?style=social&color=white)](https://github.com/tensorflow/lucid/stargazers)  
   **Neural network feature visualization and mechanistic interpretability.** Maintained historically by Google Research, Lucid provides infrastructure for generating synthetic visual inputs that maximally activate target neurons and latent channels.

8. **[LIT (Learning Interpretability Tool)](https://github.com/PAIR-code/lit)** [![GitHub_Stars](https://img.shields.io/github/stars/PAIR-code/lit?style=social&color=white)](https://github.com/PAIR-code/lit/stargazers)  
   **Google PAIR's visual interactive model debugging UI.** A visual platform for deep analysis of NLP, vision, and tabular models—supporting counterfactual generation, saliency maps, attention inspection, and slice-based fairness analysis.

9. **[TruLens](https://github.com/truera/trulens)** [![GitHub_Stars](https://img.shields.io/github/stars/truera/trulens?style=social&color=white)](https://github.com/truera/trulens/stargazers)  
   **LLM and RAG explainability & evaluation engine.** Evaluates retrieval-augmented generation pipelines using the "RAG Triad" (context relevance, groundedness, answer relevance) with programmatic feedback functions.

10. **[Shapash](https://github.com/MAIF/shapash)** [![GitHub_Stars](https://img.shields.io/github/stars/MAIF/shapash?style=social&color=white)](https://github.com/MAIF/shapash/stargazers)  
    **Human-friendly explanation dashboards.** Built by MAIF, Shapash wraps SHAP and LightGBM/XGBoost to present non-technical stakeholders with clean visual summaries, explicit feature labels, and standalone web reports.

11. **[AIF360 (AI Fairness 360)](https://github.com/Trusted-AI/AIF360)** [![GitHub_Stars](https://img.shields.io/github/stars/Trusted-AI/AIF360?style=social&color=white)](https://github.com/Trusted-AI/AIF360/stargazers)  
    **IBM's extensible algorithmic bias and fairness toolkit.** Offers over 70 fairness metrics and 10 state-of-the-art bias mitigation algorithms across pre-processing (reweighing), in-processing (adversarial debiasing), and post-processing steps.

12. **[ELI5](https://github.com/TeamHG-Memex/eli5)** [![GitHub_Stars](https://img.shields.io/github/stars/TeamHG-Memex/eli5?style=social&color=white)](https://github.com/TeamHG-Memex/eli5/stargazers)  
    **Python package for debugging ML classifiers.** Quick visualization and inspection of weights, decision trees, TextExplainer highlighting for NLP classifiers, and Permutation Importance for scikit-learn models.

13. **[whylogs](https://github.com/whylabs/whylogs)** [![GitHub_Stars](https://img.shields.io/github/stars/whylabs/whylogs?style=social&color=white)](https://github.com/whylabs/whylogs/stargazers)  
    **Statistical data profiling standard for AI pipelines.** Generates lightweight, mergeable statistical sketches of input data distributions and model predictions without copying raw data, enabling privacy-preserving drift auditing.

14. **[Alibi Explain](https://github.com/SeldonIO/alibi)** [![GitHub_Stars](https://img.shields.io/github/stars/SeldonIO/alibi?style=social&color=white)](https://github.com/SeldonIO/alibi/stargazers)  
    **Seldon's enterprise explanation library.** Specializes in Anchor explanations, Counterfactual instances ("what needs to change for the loan to be approved?"), Integrated Gradients, and trust scores.

15. **[AIX360 (AI Explainability 360)](https://github.com/Trusted-AI/AIX360)** [![GitHub_Stars](https://img.shields.io/github/stars/Trusted-AI/AIX360?style=social&color=white)](https://github.com/Trusted-AI/AIX360/stargazers)  
    **IBM's unified multi-method explainability suite.** Implements contrastive explanations, Boolean rule sets, Generalized Additive Models, and protodash prototypes for all lifecycle stages of machine learning models.

16. **[DiCE (Diverse Counterfactual Explanations)](https://github.com/interpretml/diCE)** [![GitHub_Stars](https://img.shields.io/github/stars/interpretml/diCE?style=social&color=white)](https://github.com/interpretml/diCE/stargazers)  
    **Microsoft's counterfactual explanation engine.** Generates diverse, feasible counterfactual sets showing actionable paths to change a model's prediction while satisfying feature feasibility constraints.

17. **[DALEX](https://github.com/ModelOriented/DALEX)** [![GitHub_Stars](https://img.shields.io/github/stars/ModelOriented/DALEX?style=social&color=white)](https://github.com/ModelOriented/DALEX/stargazers)  
    **Model-agnostic exploratory explainability.** Dual-ecosystem toolkit (available in Python and R) for break-down plots, variable importance measures, Ceteris Paribus curves, and fairness auditing.

18. **[TensorFlow Model Analysis (TFMA)](https://github.com/tensorflow/model-analysis)** [![GitHub_Stars](https://img.shields.io/github/stars/tensorflow/model-analysis?style=social&color=white)](https://github.com/tensorflow/model-analysis/stargazers)  
    **TFX ecosystem evaluation tool.** Evaluates models across customized slices of data, validating fairness metrics, tracking performance degradation across iterations, and spotting slice-specific blindspots.

19. **[tf-explain](https://github.com/sicara/tf-explain)** [![GitHub_Stars](https://img.shields.io/github/stars/sicara/tf-explain?style=social&color=white)](https://github.com/sicara/tf-explain/stargazers)  
    **Interpretability methods for TensorFlow 2.x and Keras.** Implements Grad-CAM, Integrated Gradients, SmoothGrad, Vanilla Gradients, and Occlusion Sensitivity with native Keras callback integrations.

20. **[What-If Tool](https://github.com/PAIR-code/what-if-tool)** [![GitHub_Stars](https://img.shields.io/github/stars/PAIR-code/what-if-tool?style=social&color=white)](https://github.com/PAIR-code/what-if-tool/stargazers)  
    **Google PAIR's visual interactive probing widget.** Seamlessly integrates into Jupyter and TensorBoard to test edge cases, probe dataset slices, and analyze algorithmic counterfactuals without writing code.

---

## 🤝 How to Contribute

Contributions are warmly welcomed! Help keep this repository comprehensive, factual, and up to date:

1. **Fork** the repository.
2. **Add or refine** tools in `README.md` (keep descriptions concise, objective, and include proper pricing/license metadata).
3. Ensure every open-source repository includes a Stars_Badge formatted as `[![GitHub_Stars](https://img.shields.io/github/stars/owner/repo?style=social&color=white)](https://github.com/owner/repo/stargazers)`.
4. Open a **Pull Request** detailing your changes.

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Machine-Learning-Interpretability&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Machine-Learning-Interpretability&type=date&legend=top-left)

---

## 💖 Support & Sponsorship

If this curated repository saved you hours of research or helps your engineering and data science teams build transparent AI systems, please consider:
- ⭐ **Starring** the repository on GitHub
- 🍴 **Forking** and contributing additional resources
- 📢 **Sharing** with your colleagues, community, and LinkedIn networks
- ☕ **Buying a coffee** via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007)

Your support keeps these developer resources active, updated, and freely accessible!

---

## ⚖️ Disclaimer

- This is an independent **community-curated** reference list—not a paid promotion or direct vendor endorsement.
- **Enterprise SaaS pricing fluctuates**: Many high-tier enterprise systems operate via customized private agreements or consumption credits. Always verify the latest pricing directly with the vendor.
- **Interpretability ≠ Fairness**: Explaining *why* a model reached a specific prediction does not guarantee the decision is non-discriminatory. Always pair attribution frameworks (e.g., SHAP, Captum) with dedicated algorithmic fairness metrics (e.g., AIF360, What-If Tool).
