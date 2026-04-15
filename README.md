<p align="center">
  <img src="llmeval-logo.png" width="200">
</p>

<h2 align="center">LLMEval-1: Large-Scale Chinese LLM Evaluation (Phase I)</h2>

<p align="center">
  <a href="https://arxiv.org/abs/2312.07398"><img src="https://img.shields.io/badge/Paper-Arxiv-blue.svg?style=for-the-badge" alt="Paper"></a>
  <a href="https://doi.org/10.1609/aaai.v38i17.29934"><img src="https://img.shields.io/badge/Venue-AAAI%202024-orange.svg?style=for-the-badge" alt="AAAI 2024"></a>
  <a href="https://github.com/llmeval"><img src="https://img.shields.io/badge/Org-LLMEval-green.svg?style=for-the-badge" alt="LLMEval"></a>
</p>

> **Note:** For the Chinese version of this README, please refer to [README_zh.md](README_zh.md).

## 🔔 News

- 🏆 **[2024-03-24]** Our paper "LLMEval: A Preliminary Study on How to Evaluate Large Language Models" has been accepted at **AAAI 2024**.
- 📊 **[2023-06-19]** Evaluation results released: 2,186 users participated, generating 243,000+ annotations.
- 🎉 **[2023-05-01]** LLMEval-1 evaluation launched.

## 📚 Overview

LLMEval-1 is the **Phase I dataset** of the [LLMEval](https://arxiv.org/abs/2312.07398) paper (AAAI 2024). It is a large-scale Chinese LLM evaluation covering **17 major categories** with **453 questions**, spanning factual QA, reading comprehension, framework generation, paragraph rewriting, summarization, mathematical problem-solving, reasoning, poetry generation, programming, and more.

### Key Features

- **Generative evaluation** — unlike multiple-choice benchmarks, models generate free-form answers
- **Five evaluation dimensions** — Correctness, Fluency, Informativeness, Logic, and Harmlessness
- **Multi-annotator evaluation** — combining onsite experts, crowd-sourcing workers, public volunteers, and GPT-4
- **2,186 participants** contributed 243,337 manual annotations
- **57,511 GPT-4** automated evaluation results

## 🏆 Leaderboard

| Model | Overall | Rank | Accuracy | Info. | Fluency | Logic | Safety | Pairwise | Rank |
|:------|:--------|:-----|:---------|:------|:--------|:------|:-------|:---------|:-----|
| GPT-4 | 2.833 (2.917) | 1 (1) | 2.709 (2.803) | 2.817 (2.882) | 2.870 (3.000) | 2.832 (2.901) | 2.937 (3.000) | 0.701 (0.894) | 1 (1) |
| GPT-3.5 | 2.789 (2.878) | 2 (2) | 2.616 (2.717) | 2.742 (2.807) | 2.850 (3.000) | 2.785 (2.868) | 2.954 (2.998) | 0.643 (0.818) | 2 (2) |
| Xunfei-Xinhuo | 2.639 (2.724) | 3 (4) | 2.391 (2.427) | 2.523 (2.564) | 2.745 (2.987) | 2.633 (2.646) | 2.904 (2.996) | 0.550 (0.623) | 5 (3) |
| Chat-Baichuan-7B | 2.633 (2.821) | 4 (3) | 2.401 (2.651) | 2.453 (2.709) | 2.720 (2.998) | 2.627 (2.753) | 2.964 (2.993) | 0.603 (0.621) | 3 (4) |
| ChatGLM-6B | 2.597 (2.644) | 5 (7) | 2.323 (2.312) | 2.504 (2.442) | 2.703 (2.956) | 2.555 (2.518) | 2.899 (2.989) | 0.579 (0.547) | 4 (5) |
| Chinese-LLAMA-7B | 2.571 (2.723) | 6 (5) | 2.293 (2.431) | 2.394 (2.549) | 2.696 (2.993) | 2.553 (2.646) | 2.919 (2.998) | 0.506 (0.457) | 6 (7) |
| Ali-Tongyiqianwen | 2.523 (2.646) | 7 (6) | 2.203 (2.309) | 2.339 (2.403) | 2.670 (2.983) | 2.530 (2.542) | 2.875 (2.991) | 0.491 (0.507) | 7 (6) |
| NewBing | 2.464 (2.622) | 8 (8) | 2.127 (2.263) | 2.144 (2.320) | 2.607 (2.996) | 2.550 (2.531) | 2.892 (2.998) | 0.415 (0.425) | 9 (8) |
| MOSS-16B | 2.337 (2.518) | 9 (10) | 1.994 (2.109) | 2.054 (2.173) | 2.498 (2.974) | 2.288 (2.370) | 2.849 (2.965) | 0.377 (0.272) | 11 (10) |
| Linly-ChatFlow-13B | 2.312 (2.534) | 11 (9) | 1.966 (2.158) | 2.067 (2.257) | 2.408 (2.928) | 2.288 (2.351) | 2.830 (2.976) | 0.398 (0.339) | 10 (9) |
| ChatYuan-Large | 2.312 (2.411) | 11 (12) | 1.933 (1.961) | 2.095 (2.056) | 2.458 (2.851) | 2.247 (2.195) | 2.826 (2.994) | 0.426 (0.245) | 8 (12) |
| MOSS-w-Plugin-16B | 2.310 (2.506) | 12 (11) | 1.966 (2.101) | 1.964 (2.150) | 2.499 (2.963) | 2.285 (2.352) | 2.834 (2.967) | 0.352 (0.254) | 12 (11) |

*Values in parentheses are GPT-4 automated evaluation scores and rankings.*

## 🔗 Related Projects

| Project | Description | Link |
|---------|-------------|------|
| **LLMEval** (AAAI 2024) | Main paper with methodology and analysis | [arXiv](https://arxiv.org/abs/2312.07398) |
| **LLMEval-2** | Phase II: Professional domain evaluation | [GitHub](https://github.com/llmeval/LLMEval-2) |
| **LLMEval-Fair** (ACL 2026) | Robust & fair evaluation, 200K+ questions | [GitHub](https://github.com/llmeval/LLMEval-Fair) |
| **LLMEval-Med** (EMNLP 2025) | Medical LLM benchmark | [GitHub](https://github.com/llmeval/LLMEval-Med) |
| **Official Website** | All projects & leaderboard | [llmeval.com](http://llmeval.com/) |

## 📝 Citation

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

## 📞 Contact Us

This project is open to the public, and we welcome you to participate in our evaluation.

- **Website**: [http://llmeval.com/](http://llmeval.com/)
- **Email**: mingzhang23@m.fudan.edu.cn
- **WeChat**: zanyingluan

---

<p align="center">
  <b>LLMEval</b> | Fudan University NLP Lab
</p>
