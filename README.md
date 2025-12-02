<div align="center">

# Multi-Personality Generation of LLMs at Decoding-time

[![WSDM 2026](https://img.shields.io/badge/WSDM-2026-4b44ce.svg?style=flat-square)](https://www.wsdm-conference.org/)
[![ArXiv](https://img.shields.io/badge/ArXiv-2511.01891-b31b1b.svg?style=flat-square)](http://arxiv.org/abs/2511.01891)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Datasets-blue?style=flat-square)](https://huggingface.co/RongxinChen)

**Rongxin Chen, Yunfan Li, Yige Yuan, Bingbing Xu, Huawei Shen**

</div>

---

## 📖 Abstract

Multi-personality generation for LLMs, enabling simultaneous embodiment of multiple personalization attributes, is a fundamental challenge. Existing retraining-based approaches are costly and poorly scalable, while decoding-time methods often rely on external models or heuristics, limiting flexibility and robustness. 

In this paper, we propose a novel **Multi-Personality Generation (MPG)** framework under the decoding-time combination paradigm. It flexibly controls multi-personality without relying on scarce multi-dimensional models or extra training, leveraging implicit density ratios in single-dimensional models as a "free lunch" to reformulate the task as sampling from a target strategy aggregating these ratios. To implement MPG efficiently, we design **Speculative Chunk-level based Rejection sampling (SCR)**, which generates responses in chunks and parallelly validates them via estimated thresholds within a sliding window. This significantly reduces computational overhead while maintaining high-quality generation. Experiments on MBTI personality and Role-Playing demonstrate the effectiveness of MPG, showing improvements up to **16%-18%**.

## 🚀 Highlights

- **MPG Framework**: A decoding-time combination paradigm that requires **no extra training** or multi-dimensional models.
- **SCR Algorithm**: Uses **Speculative Chunk-level Rejection sampling** to parallelly validate generated chunks, significantly reducing computational overhead.
- **High Performance**: Achieves up to **18% improvement** on MBTI and Role-Playing benchmarks compared to existing methods.

## 📚 Datasets

We release the **MBTI** and **RolePlay** DPO (Direct Preference Optimization) datasets used in our study.

### 🧩 MBTI Datasets
These datasets focus on specific Myers-Briggs Type Indicator dimensions.

| Dimension | Description | Dataset Link |
| :--- | :--- | :--- |
| **E / I** | Extraversion vs. Introversion | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/MBTI_dpo_e_i) |
| **J / P** | Judging vs. Perceiving | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/MBTI_dpo_j_p) |
| **T / F** | Thinking vs. Feeling | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/MBTI_dpo_t_f) |
| **S / N** | Sensing vs. Intuition | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/MBTI_dpo_s_n) |

### 🎭 RolePlay Datasets
Datasets designed for enhancing role-playing capabilities.

| Type | Description | Dataset Link |
| :--- | :--- | :--- |
| **Personality** | DPO data for general personality alignment | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/dpo_personality) |
| **Profile** | DPO data based on character profiles | [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Open%20in%20HF-blue)](https://huggingface.co/datasets/RongxinChen/dpo_profile) |

## 🖊️ Citation

If you find our work or datasets useful, please consider citing our paper:

```bibtex
@inproceedings{chen2026multipersonality,
  title={Multi-Personality Generation of LLMs at Decoding-time},
  author={Chen, Rongxin and Li, Yunfan and Yuan, Yige and Xu, Bingbing and Shen, Huawei},
  booktitle={Proceedings of the 19th ACM International Conference on Web Search and Data Mining (WSDM '26)},
  year={2026},
  publisher={ACM},
  url={http://arxiv.org/abs/2511.01891}
}
