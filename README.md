# Shell@Educhat: Benchmark for Implicit Value Risk Mining and Alignment in Domain-Specific LLMs

<div align="center">

[![Paper](https://img.shields.io/badge/Paper-Arxiv-red)](https://arxiv.org/abs/2511.07107)
[![Project Page](https://img.shields.io/badge/Project-Website-green)](https://feifeinoban.huggingface.co/spaces/feifeinoban/shell)
[![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/KCshen1125/Shell-Safety-Benchmark/blob/main/LICENSE)

[English](README.md) | [中文](README_zh.md)

</div>

## 🚀 News

- **[2025-12-25]** The [Project Page](https://feifeinoban.huggingface.co/spaces/feifeinoban/shell) is live, and the paper is available on ArXiv.
- **[Coming Soon]** The **Domain Implicit Risk Dataset** and the **MENTOR** framework code are currently being organized and will be released shortly. Please star ⭐ this repository for the latest updates!

---

## 📖 Introduction

**Shell** is a benchmark and framework dedicated to uncovering and mitigating **Implicit Risks** in domain-specific Large Language Models (LLMs). Unlike general safety benchmarks that focus on explicit harms (e.g., violence, hate speech), Shell focuses on deep-seated, context-dependent risks in vertical domains such as **Education**, **Finance**, and **Management**.

We introduce:
1.  **Domain Safety Dataset**: Categorizes risks into Green (Guide), Yellow (Reflect), and Red (Deny).
2.  **MENTOR Framework**: A self-evolving safety mechanism using a Rule Evolution Cycle (REC) and Activation Steering (RV) to effectively detect and mitigate these subtle risks.

## 📊 Dataset Evaluation

The dataset focuses on the "Litmus Strip" framework, identifying risks hidden beneath the surface of professional queries.

| Domain | Focus Areas | Risk Examples |
| :--- | :--- | :--- |
| **Education** | Student Psychology, Academic Pressure | Encouraging extreme sacrifice for grades, Inducing excessive involution |
| **Management** | Recruitment, Organizational Behavior | Implicit discrimination, Unethical incentives, Improper benefit transfer |
| **Finance** | Investment Advice, Sales Tactics | Misleading high-yield promises, Malicious competitor defamation |

## 🛠️ MENTOR Framework

MENTOR is designed to be a "Guardian" for domain-specific models:

* **REC (Rule Evolution Cycle):** A metacognition-driven feedback loop that continuously discovers and summarizes new risk response rules.
* **RV (Rule Vector):** Utilizes Activation Steering to directly intervene in the model's internal representation, allowing the model to "internalize" safety constraints.

## 🗓️ Roadmap

- [x] Release Paper and Project Page.
- [ ] Release **Domain Safety Dataset** (Evaluation Data).
- [ ] Release **MENTOR** training and inference code.

## 📝 Citation

If you find our work useful, please cite our paper:

```bibtex
@article{shell2025mentor,
  title={MENTOR: A Metacognition-Driven Self-Evolution Framework for Uncovering and Mitigating Implicit Risks in LLMs on Domain Tasks},
  author={Shell@Educhat Team},
  journal={arXiv preprint arXiv:2511.07107},
  year={2025}
}
