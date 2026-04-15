<p align="center">
  <img src="llmeval-logo.png" width="200">
</p>

<h2 align="center">LLMEval-1: 中文大语言模型评测第一期</h2>

<p align="center">
  <a href="https://arxiv.org/abs/2312.07398"><img src="https://img.shields.io/badge/论文-Arxiv-blue.svg?style=for-the-badge" alt="论文"></a>
  <a href="https://doi.org/10.1609/aaai.v38i17.29934"><img src="https://img.shields.io/badge/会议-AAAI%202024-orange.svg?style=for-the-badge" alt="AAAI 2024"></a>
  <a href="https://github.com/llmeval"><img src="https://img.shields.io/badge/组织-LLMEval-green.svg?style=for-the-badge" alt="LLMEval"></a>
</p>

> **注意：** 英文版 README 请参阅 [README.md](README.md)。

## 🔔 最新消息

- 🏆 **[2024-03-24]** 论文 "LLMEval: A Preliminary Study on How to Evaluate Large Language Models" 被 **AAAI 2024** 录用。
- 📊 **[2023-06-19]** 评测结果发布：2,186 位用户参与，生成 24.3 万条标注数据。
- 🎉 **[2023-05-01]** LLMEval-1 评测正式上线。

## 📚 项目简介

LLMEval-1 是 [LLMEval](https://arxiv.org/abs/2312.07398)（AAAI 2024）论文的**第一期评测数据集**。本评测涵盖了 **17 个大类**、**453 个问题**，包括事实性问答、阅读理解、框架生成、段落重写、摘要、数学解题、推理、诗歌生成、编程等各个领域。

### 核心特点

- **生成式评测** — 不同于选择题基准，模型需要生成自由文本回答
- **五大评价维度** — 正确性、流畅性、信息量、逻辑性、无害性
- **多类评估者** — 现场专家 + 众包标注员 + 公众志愿者 + GPT-4 自动评测
- **2,186 名参与者**贡献了 243,337 条人工标注
- **57,511 条 GPT-4** 自动评测结果

## 🏆 排行榜

| 模型名称 | 综合 | 排名 | 准确率 | 信息量 | 流畅性 | 逻辑性 | 无害性 | 对比打分 | 排名 |
|:---------|:-----|:-----|:-------|:-------|:-------|:-------|:-------|:---------|:-----|
| GPT-4 | 2.833 (2.917) | 1 (1) | 2.709 (2.803) | 2.817 (2.882) | 2.870 (3.000) | 2.832 (2.901) | 2.937 (3.000) | 0.701 (0.894) | 1 (1) |
| GPT-3.5 | 2.789 (2.878) | 2 (2) | 2.616 (2.717) | 2.742 (2.807) | 2.850 (3.000) | 2.785 (2.868) | 2.954 (2.998) | 0.643 (0.818) | 2 (2) |
| 讯飞星火 | 2.639 (2.724) | 3 (4) | 2.391 (2.427) | 2.523 (2.564) | 2.745 (2.987) | 2.633 (2.646) | 2.904 (2.996) | 0.550 (0.623) | 5 (3) |
| Chat-Baichuan-7B | 2.633 (2.821) | 4 (3) | 2.401 (2.651) | 2.453 (2.709) | 2.720 (2.998) | 2.627 (2.753) | 2.964 (2.993) | 0.603 (0.621) | 3 (4) |
| ChatGLM-6B | 2.597 (2.644) | 5 (7) | 2.323 (2.312) | 2.504 (2.442) | 2.703 (2.956) | 2.555 (2.518) | 2.899 (2.989) | 0.579 (0.547) | 4 (5) |
| Chinese-LLAMA-7B | 2.571 (2.723) | 6 (5) | 2.293 (2.431) | 2.394 (2.549) | 2.696 (2.993) | 2.553 (2.646) | 2.919 (2.998) | 0.506 (0.457) | 6 (7) |
| 通义千问 | 2.523 (2.646) | 7 (6) | 2.203 (2.309) | 2.339 (2.403) | 2.670 (2.983) | 2.530 (2.542) | 2.875 (2.991) | 0.491 (0.507) | 7 (6) |
| NewBing | 2.464 (2.622) | 8 (8) | 2.127 (2.263) | 2.144 (2.320) | 2.607 (2.996) | 2.550 (2.531) | 2.892 (2.998) | 0.415 (0.425) | 9 (8) |
| MOSS-16B | 2.337 (2.518) | 9 (10) | 1.994 (2.109) | 2.054 (2.173) | 2.498 (2.974) | 2.288 (2.370) | 2.849 (2.965) | 0.377 (0.272) | 11 (10) |
| Linly-ChatFlow-13B | 2.312 (2.534) | 11 (9) | 1.966 (2.158) | 2.067 (2.257) | 2.408 (2.928) | 2.288 (2.351) | 2.830 (2.976) | 0.398 (0.339) | 10 (9) |
| ChatYuan-Large | 2.312 (2.411) | 11 (12) | 1.933 (1.961) | 2.095 (2.056) | 2.458 (2.851) | 2.247 (2.195) | 2.826 (2.994) | 0.426 (0.245) | 8 (12) |
| MOSS-w-Plugin-16B | 2.310 (2.506) | 12 (11) | 1.966 (2.101) | 1.964 (2.150) | 2.499 (2.963) | 2.285 (2.352) | 2.834 (2.967) | 0.352 (0.254) | 12 (11) |

*注：括号内数值为 GPT-4 自动评测的打分及排名。*

## 🔗 相关项目

| 项目 | 说明 | 链接 |
|------|------|------|
| **LLMEval**（AAAI 2024） | 主论文，包含方法论与分析 | [arXiv](https://arxiv.org/abs/2312.07398) |
| **LLMEval-2** | 第二期：专业领域评测 | [GitHub](https://github.com/llmeval/LLMEval-2) |
| **LLMEval-Fair**（ACL 2026） | 鲁棒公平评测，20 万+题 | [GitHub](https://github.com/llmeval/LLMEval-Fair) |
| **LLMEval-Med**（EMNLP 2025） | 医学大模型基准 | [GitHub](https://github.com/llmeval/LLMEval-Med) |
| **官方网站** | 全部项目与排行榜 | [llmeval.com](http://llmeval.com/) |

## 📝 引用

```bibtex
@inproceedings{zhang2024llmeval,
  title     = {LLMEval: A Preliminary Study on How to Evaluate Large Language Models},
  author    = {Yue Zhang and Ming Zhang and Haipeng Yuan and Shichun Liu and Yongyao Shi and Tao Gui and Qi Zhang and Xuanjing Huang},
  booktitle = {Proceedings of the AAAI Conference on Artificial Intelligence},
  volume    = {38},
  number    = {17},
  pages     = {19615--19622},
  year      = {2024},
  doi       = {10.1609/aaai.v38i17.29934}
}
```

## 📞 联系我们

本项目已经向公众开放，欢迎参与我们的评测。

- **网站**：[http://llmeval.com/](http://llmeval.com/)
- **邮箱**：mingzhang23@m.fudan.edu.cn
- **微信**：zanyingluan

---

<p align="center">
  <b>LLMEval</b> | 复旦大学 NLP 实验室
</p>
