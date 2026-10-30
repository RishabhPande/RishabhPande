# Rishabh Pande

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishabhpande/)
[![ORCID](https://img.shields.io/badge/ORCID-iD-A6CE39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0004-1901-7109)
![Peer Reviewer](https://img.shields.io/badge/Peer_Reviewer-IEEE_Access_%7C_KBS-00629B?style=flat-square)

**Sr. Director of Data Science @ Socure.** I lead ML teams building real-time fraud and risk machine learning models operating at massive scale.

My work lives at the intersection of **AI, neural networks, and transformer models**: anomaly detection, identity verification, and catching coordinated fraud attacks, synthetic identities, and adversarial abuse in real-time transaction streams.

## See it run

<p align="center"><a href="https://github.com/RishabhPande/agentstats"><img src="https://raw.githubusercontent.com/RishabhPande/agentstats/main/docs/leaderboard_uncertainty.png" alt="Ten repeated runs of the same 12 agent configurations on SWE-bench Verified: the top spot changes between runs" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/agentstats">agentstats</a></b>: Ten repeated runs of the same 12 agent configurations. Two statistically tied agents swap first place, so a single published run can crown either one. Real data from ASSERT-KTH (CC-BY-4.0).</sub></p>

<p align="center"><a href="https://github.com/RishabhPande/fraud-rings"><img src="https://raw.githubusercontent.com/RishabhPande/fraud-rings/main/docs/rings.png" alt="Fraud rings found by exact address match versus normalized address match" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/fraud-rings">fraud-rings</a></b>: Address normalization recovers 2 of 3 planted rings that exact matching misses. The ring spread across several apartment units stays split on purpose. Synthetic data.</sub></p>

<p align="center"><a href="https://github.com/RishabhPande/stream-fraud"><img src="https://raw.githubusercontent.com/RishabhPande/stream-fraud/main/docs/drift_replay.png" alt="Drift replay: rolling score, PSI and KS statistics, and alarm delays over 20 seeds" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/stream-fraud">stream-fraud</a></b>: Drift replay over 20 seeds. PSI alarmed earlier than a KS test here, and neither is false-alarm free. Synthetic data.</sub></p>

## Projects

**Evaluation, statistics and benchmarks**

| Repo | What it is |
|------|------------|
| [agentstats](https://github.com/RishabhPande/agentstats) | Run-to-run variance, significance tests and minimum-runs planning for AI agent benchmarks. Install from Git (the PyPI name belongs to another package). |
| [fraud-eval](https://github.com/RishabhPande/fraud-eval) | Open benchmark for LLM-based fraud and abuse detectors. v0.1.0 is a 20-case smoke test with a Hugging Face dataset and leaderboard. |
| [agentrisk](https://github.com/RishabhPande/agentrisk) | Benchmark and code for the preprint "Automation Is Not Intent": how fraud models treat legitimate AI shopping agents. |
| [feature-contracts](https://github.com/RishabhPande/feature-contracts) | Reproduction package for the feature-contracts manuscript, using public datasets. |

**Fraud and anomaly detection, from scratch in pure Python (synthetic data)**

| Repo | What it is |
|------|------------|
| [GNN-fraud-ring-detection](https://github.com/RishabhPande/GNN-fraud-ring-detection) | GraphSAGE, GAT and other graph networks with no dependencies, applied to fraud rings in transaction networks. |
| [fraud-rings](https://github.com/RishabhPande/fraud-rings) | Synthetic ring generator plus shared-attribute linking with union-find. |
| [stream-fraud](https://github.com/RishabhPande/stream-fraud) | Streaming scoring pipeline demo: velocity features, rule-based scorer, PSI and KS drift detection. |
| [Time-series-anomaly-detection](https://github.com/RishabhPande/Time-series-anomaly-detection) | Transformer autoencoder for collective and contextual anomalies. |
| [ID-document-forgery-detection-CV-](https://github.com/RishabhPande/ID-document-forgery-detection-CV-) | Classic image forensics on synthetic ID cards with planted forgeries. |
| [agentic-fraud-investigator](https://github.com/RishabhPande/agentic-fraud-investigator) | Multi-agent case investigation: triage, evidence, risk score, analyst-style report. Runs offline with a mock LLM by default. |

**Agents**

| Repo | What it is |
|------|------------|
| [know-your-agent](https://github.com/RishabhPande/know-your-agent) | Offline prototype of scoped, session-limited, revocable agent credentials signed with Ed25519. An audit trail is planned, not built. |
| [agent-retry-rodeo](https://github.com/RishabhPande/agent-retry-rodeo) | Local test range for agent recovery: watch "done" fail against a fault, then replay a recovery-aware baseline. |

**Learning**

| Repo | What it is |
|------|------------|
| [tiny-ml-lab](https://github.com/RishabhPande/tiny-ml-lab) | One classic ML algorithm a day, numpy only, with a workbook to fill in. |

Presented as separate projects; no integrated pipeline is claimed here.

## Research & service

- **Paper:** "Counterfactual Evaluation of Fraud Models under Selective and Delayed Labels", submitted to TMLR, (Transactions on Machine Learning Research), Oct 2026
- Peer reviewer: **IEEE Access**, **Knowledge-Based Systems** (Elsevier)
- Program Committee: **IJCNN 2027**
- Co-inventor on pending patent applications in AI-driven fraud detection (US + EP)

## Connect

- [LinkedIn](https://www.linkedin.com/in/rishabhpande/)
- [ORCID](https://orcid.org/0009-0004-1901-7109)

*Currently building in public. New commits land daily.*
