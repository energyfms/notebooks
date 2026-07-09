<div align="center">

# EnergyFM

### Pretrained Time Series Foundation Models for Energy Meter Data Analytics

[![Paper](https://img.shields.io/badge/Paper-ACM%20e--Energy%202026-B31B1B)](https://doi.org/10.1145/3744255.3798119)
[![Website](https://img.shields.io/badge/Website-EnergyFM-2ea44f)](https://energyfms.github.io/)
[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Models-FFD21E)](https://huggingface.co/EnergyFM)
[![Leaderboard](https://img.shields.io/badge/Leaderboard-EnergyBench-blue)](https://huggingface.co/spaces/EnergyFM/Leaderboard)

**Quick Links**
[Website](https://energyfms.github.io/) •
[Paper](https://doi.org/10.1145/3744255.3798119) •
[Hugging Face](https://huggingface.co/EnergyFM) •
[Leaderboard](https://huggingface.co/spaces/EnergyFM/Leaderboard) •
[Energy-TTM](https://huggingface.co/EnergyFM/energy-ttm) •
[Energy-TSPulse](https://huggingface.co/EnergyFM/energy-tspulse)

</div>

---



## 📖 Introduction

**EnergyFM** is a suite of **pretrained time series foundation models (TSFMs)** for **energy meter data analytics**. It provides pretrained models, example pipelines, and tutorial notebooks for **short-term load forecasting, anomaly detection, and appliance classification** on large-scale smart meter datasets.

EnergyFM is designed to support:

* **Zero-shot inference** on unseen buildings and regions
* **Fine-tuning** for downstream energy analytics tasks
* **Reproducible benchmarking** across forecasting and representation-learning tasks

This repository accompanies the paper:

> **EnergyFM: Pretrained Models for Energy Meter Data Analytics**
> *ACM e-Energy 2026*

---

## ⚡ Models

EnergyFM currently includes two pretrained models, each targeting a different class of energy analytics tasks:

| Model              | Architecture          | Primary Use             | Supported Tasks                             |
| ------------------ | --------------------- | ----------------------- | ------------------------------------------- |
| **Energy-TTM**     | Tiny Time Mixer (TTM) | Forecasting             | Short-term load forecasting                 |
| **Energy-TSPulse** | TSPulse               | Representation learning | Anomaly detection, appliance classification |

---

## 🌍 Multi-Task Evaluation 

To compare EnergyFM against other state-of-the-art time series foundation models for energy analytics, visit our public leaderboard:

👉 **[Energy Multi-Task Leaderboard](https://huggingface.co/spaces/EnergyFM/Leaderboard)**

The leaderboard provides standardized evaluations across multiple energy forecasting, anomaly detection, and classification tasks, allowing direct comparison between EnergyFM and other TSFMs under consistent evaluation settings.

---

## 🧑‍💻 Installation

Clone the repository:

```bash id="74otj1"
git clone https://github.com/energyfms/notebooks.git
cd notebooks
```

Install dependencies:

```bash id="5o8r0m"
pip install -r requirements.txt
```

---

## 🚀 Getting Started

### Energy-TTM

| Tutorial | GitHub | Colab |
|----------|--------|--------|
| **Zero-Shot Forecasting** | [Notebook](https://github.com/energyfms/notebooks/blob/main/energy_ttm_zeroshot.ipynb) | <a target="_blank" href="https://colab.research.google.com/github/energyfms/notebooks/blob/main/energy_ttm_zeroshot.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| **Fine-Tuning for Forecasting** | [Notebook](https://github.com/energyfms/notebooks/blob/main/energy_ttm_finetuning.ipynb) | <a target="_blank" href="https://colab.research.google.com/github/energyfms/notebooks/blob/main/energy_ttm_finetuning.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |

### Energy-TSPulse

| Tutorial | GitHub | Colab |
|----------|--------|--------|
| **Zero-Shot Anomaly Detection** | [Notebook](https://github.com/energyfms/notebooks/blob/main/energy_tspulse_anomaly_detection_zeroshot.ipynb) | <a target="_blank" href="https://colab.research.google.com/github/energyfms/notebooks/blob/main/energy_tspulse_anomaly_detection_zeroshot.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| **Fine-Tuning for Anomaly Detection** | [Notebook](https://github.com/energyfms/notebooks/blob/main/energy_tspulse_anomaly_detection_finetuning.ipynb) | <a target="_blank" href="https://colab.research.google.com/github/energyfms/notebooks/blob/main/energy_tspulse_anomaly_detection_finetuning.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
| **Appliance Classification (Fine-Tuning)** | [Notebook](https://github.com/energyfms/notebooks/blob/main/energy_tspulse_classification_finetuning.ipynb) | <a target="_blank" href="https://colab.research.google.com/github/energyfms/notebooks/blob/main/energy_tspulse_classification_finetuning.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> |
---

## 🤗 Pretrained Models

Pretrained checkpoints and model cards are hosted on Hugging Face:

* **Energy-TTM** — forecasting model for short-term load forecasting
  [View Model Card](https://huggingface.co/EnergyFM/energy-ttm)

* **Energy-TSPulse** — representation model for anomaly detection and appliance classification
  [View Model Card](https://huggingface.co/EnergyFM/energy-tspulse)

---

## 🔧 Dependencies

EnergyFM builds on IBM’s **Granite Time Series Foundation Models (TSFM)** ecosystem, which provides the core model implementations and Hugging Face integration.

* **Granite TSFM GitHub:** [ibm-granite/granite-tsfm](https://github.com/ibm-granite/granite-tsfm)
* **Granite TSFM Wiki:** [Granite TSFM Wiki](https://github.com/ibm-granite/granite-tsfm/wiki)

---

## 📂 Datasets

This repository does **not** host the full pretraining or evaluation datasets.

* Small sample datasets may be included for demonstration and tutorials
* Full datasets used in the paper are released separately
* Links to datasets and pretrained weights are provided through the project website and Hugging Face model cards

---

## 📝 Citation

If you use EnergyFM in your research, please cite:

```bibtex"
@inproceedings{energyfm,
  author    = {Arjunan, Pandarasamy and Srivastava, Naman and Kumar, Kajeeth and Jati, Arindam and Ekambaram, Vijay and Dayama, Pankaj},
  title     = {EnergyFM: Pretrained Models for Energy Meter Data Analytics},
  year      = {2026},
  isbn      = {9798400720116},
  publisher = {Association for Computing Machinery},
  address   = {New York, NY, USA},
  url       = {https://doi.org/10.1145/3744255.3798119},
  doi       = {10.1145/3744255.3798119},
  booktitle = {Proceedings of the 17th ACM International Conference on Future and Sustainable Energy Systems},
  pages     = {556--568},
  series    = {E-Energy '26}
}
```

---

## ❓ Issues and Support

Please report bugs, feature requests, or questions via GitHub Issues:

https://github.com/energyfm/notebooks/issues
