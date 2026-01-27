# Shell@Educhat: Benchmark for Implicit Value Risk Mining and Alignment in Domain-Specific LLMs

<div align="center">

[![Paper](https://img.shields.io/badge/Paper-Arxiv-red)](https://arxiv.org/abs/2511.07107)
[![Hugging Face Datasets](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Datasets-yellow)](https://huggingface.co/datasets/feifeinoban/Shell)
[![Project Page](https://img.shields.io/badge/Project-Website-green)](https://feifeinoban.huggingface.co/spaces/feifeinoban/shell)
[![Demo Download](https://img.shields.io/badge/Download-Single_Instance_Demo_(Google_Drive)-blue?logo=google-drive&logoColor=white)](https://drive.google.com/file/d/1-Lm5ke1cZHABzmbHm8eFckijFt30l7Jv/view?usp=drive_link)
[![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/KCshen1125/Shell-Safety-Benchmark/blob/main/LICENSE)

[English](README.md) | [中文](README_zh.md)

</div>

## 🚀 News

- **[2026-01-27]** 🎉 **Double Release!**
    - 📊 The **Domain Safety Dataset** is now officially available on [Hugging Face](https://huggingface.co/datasets/feifeinoban/Shell).
    - 📥 The **Single-Instance Test Demo** is released via [Google Drive](https://drive.google.com/file/d/1-Lm5ke1cZHABzmbHm8eFckijFt30l7Jv/view?usp=drive_link). This demo allows for detailed analysis of individual queries.
- **[2025-12-25]** The Project Page is live, and the paper is available on ArXiv.
- **[Coming Soon]** The **MENTOR** framework code is currently being organized and will be released shortly.

---

## 💻 Demo Usage

> **⚠️ Prerequisites**
> Before running the demo, please ensure you have obtained valid API keys from:
> * **DeepSeek Official Website**
> * **Qwen (Aliyun Bailian Platform)**

**Supported Configurations:**
* **Agent Base Models:** The demo currently supports **DeepSeek** and **Qwen** as the underlying agent backbones.
* **Evaluation Targets:** The benchmark is configured to test the following three models:
    * **DeepSeek-R1**
    * **Qwen-Plus**
    * **GPT-4o**

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
- [x] Release **Single-Instance Test Demo** (via Google Drive).
- [x] Release **Domain Safety Dataset** (on Hugging Face).
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
