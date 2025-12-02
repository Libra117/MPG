<div align="center">

# Multi-Personality Generation of LLMs at Decoding-time

[![WSDM 2026](https://img.shields.io/badge/WSDM-2026-4b44ce.svg?style=flat-square)](https://www.wsdm-conference.org/)
[![ArXiv](https://img.shields.io/badge/ArXiv-2511.01891-b31b1b.svg?style=flat-square)](http://arxiv.org/abs/2511.01891)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Datasets-blue?style=flat-square)](https://huggingface.co/RongxinChen)

</div>

---

## 📖 Abstract

This repository contains the datasets and resources for the paper **"Multi-Personality Generation of LLMs at Decoding-time"**, accepted at **WSDM 2026**.

> [!NOTE]
> The abstract and further details of the methodology will be updated shortly. Please refer to the [ArXiv paper](http://arxiv.org/abs/2511.01891) for the full manuscript.

## 📚 Datasets

We release the **MBTI** and **RolePlay** DPO (Direct Preference Optimization) datasets used in our study. You can access them directly via Hugging Face.

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
@inproceedings{yourname2026multipersonality,
  title={Multi-Personality Generation of LLMs at Decoding-time},
  author={Author One and Author Two and Author Three},
  booktitle={Proceedings of the 19th ACM International Conference on Web Search and Data Mining (WSDM '26)},
  year={2026},
  url={[http://arxiv.org/abs/2511.01891](http://arxiv.org/abs/2511.01891)}
}
