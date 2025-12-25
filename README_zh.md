# Shell@Educhat: 大语言模型垂域任务隐式价值观风险挖掘与对齐基准

<div align="center">

<img src="https://img.shields.io/badge/ECNU-Data_Science-blue" alt="ECNU">
<img src="https://img.shields.io/badge/Shanghai-AI_Lab-blue" alt="Shanghai AI Lab">

[![Paper](https://img.shields.io/badge/Paper-Arxiv-red)](https://arxiv.org/abs/2511.07107)
[![Project Page](https://img.shields.io/badge/Project-Website-green)](https://feifeinoban.huggingface.co/spaces/feifeinoban/shell)
[![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://github.com/KCshen1125/Shell-Safety-Benchmark/blob/main/LICENSE)

[English](README.md) | [中文](README_zh.md)

</div>

## 🚀 最新动态

- **[2025-12-25]** 项目主页 [Project Page](https://feifeinoban.huggingface.co/spaces/feifeinoban/shell) 已上线，论文已发布于 ArXiv。
- **[敬请期待]** 垂域隐式风险 **数据集** 以及 **MENTOR** 框架代码正在整理中，稍后即将开源。欢迎 Star ⭐ 本仓库关注最新进展！

---

## 📖 简介

**Shell** 是一个致力于挖掘和缓解特定领域大语言模型（LLMs）**隐性风险（Implicit Risks）** 的评测基准与框架。与关注显性危害（如暴力、仇恨言论）的通用安全基准不同，Shell 聚焦于**教育**、**金融**和**管理**等垂直领域中深层且依赖语境的隐性风险。

我们提出了：
1.  **领域安全数据集**：将风险分为绿色（引导）、黄色（反思）和红色（拒答）三类。
2.  **MENTOR 框架**：一种自进化的安全机制，利用规则演化循环（REC）和激活引导（RV）技术，有效发现并缓解这些不易察觉的潜在风险。

## 📊 数据集评估

该数据集基于“试纸（Litmus Strip）”框架，识别深埋于专业查询表面之下的隐患。

| 领域 | 关注重点 | 风险示例 |
| :--- | :--- | :--- |
| **教育 (Education)** | 学生心理、学业压力 | 鼓励为成绩做出极端牺牲、过度内卷诱导 |
| **管理 (Management)** | 招聘选拔、组织行为 | 隐性歧视、不道德的激励机制、利益输送建议 |
| **金融 (Finance)** | 投资建议、销售话术 | 误导性高收益承诺、恶意诋毁竞争对手 |

## 🛠️ MENTOR 框架

MENTOR 旨在成为垂域大模型的“守护者”：

* **REC (规则演化循环)**：一种元认知驱动的反馈循环，持续发现并总结新的风险响应规则。
* **RV (规则向量)**：利用激活引导技术直接干预模型的内部表征，使模型能够“内化”安全约束。

## 🗓️ 路线图 (Roadmap)

- [x] 发布论文和项目主页
- [ ] 发布 **领域安全数据集** (评估数据)
- [ ] 发布 **MENTOR** 训练与推理代码
- [ ] 发布 "Judger" (评估器) 脚本

## 📝 引用

如果您觉得我们的工作对您有帮助，请引用我们的论文：

```bibtex
@article{shell2025domain,
  title={Shell@Educhat: Uncovering and Mitigating Implicit Risks in Domain-Specific LLMs},
  author={Shell@Educhat Team},
  journal={arXiv preprint arXiv:2511.07107},
  year={2025}
}
