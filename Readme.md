# EnergyFM

EnergyFM are **pretrained time series foundation models**
applied to **energy meter data**. It provides pretrained models, example pipelines,
and tutorial notebooks for **forecasting, anomaly detection, and classification**
on large-scale smart meter datasets.

EnergyFM is designed to support:
- Zero-shot inference on unseen buildings and regions
- Fine-tuning for downstream energy analytics tasks
- Reproducible research and benchmarking

This repository accompanies the paper:

**EnergyFM: Pretrained Models for Energy Meter Data Analytics**  
*ACM e-Energy 2026*

---

## Models Included

EnergyFM currently includes two pretrained models, each designed for a distinct
class of energy time series tasks.

| Model | Primary Use | Supported Tasks |
|------|------------|-----------------|
| **Energy-TTM** | Forecasting | Short-term load forecasting |
| **Energy-TSPulse** | Representation learning | Classification, anomaly detection |


---

## Installation

Clone the repository:

```bash
git clone https://github.com/energyfms/notebooks.git
cd notebooks
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Getting Started

- **Zero-Shot Forecasting with Energy-TTM**  
  [Open Notebook](https://github.com/energyfms/notebooks/blob/main/energy_ttm_zeroshot.ipynb)

- **Zero-Shot Anomaly Detection with Energy-TSPulse**  
  [Open Notebook](https://github.com/energyfms/notebooks/blob/main/energy-tspulse_anomaly_detection_zeroshot.ipynb)

- **Fine-Tuning Energy-TSPulse for Anomaly Detection**  
  [Open Notebook](https://github.com/energyfms/notebooks/blob/main/energy_tspulse_anomaly_detection_finetune.ipynb)

- **Appliance Classification with Energy-TSPulse (Fine-Tuning)**  
  [Open Notebook](https://github.com/energyfms/notebooks/blob/main/energy_tspulse_classification_finetuning.ipynb)

- **Fine-Tuning Energy-TTM for Forecasting**  
  [Open Notebook](https://github.com/energyfms/notebooks/blob/main/energy_ttm-finetuning.ipynb)

---

---

## Datasets

This repository does **not** host full datasets.

* Small samples may be included for demonstration purposes
* Full datasets used for pretraining and evaluation are released separately

Links to datasets and pretrained weights are provided via Hugging Face.


---

## Issues

Please report bugs or questions via GitHub Issues:

[https://github.com/energyfms/notebooks/issues](https://github.com/energyfms/notebooksissues)

---

## Citation

If you use EnergyFM in your research, please cite:

```bibtex
@article{energyfm2026,
  title   = {EnergyFM: Pretrained Models for Energy Meter Data Analytics},
  author  = {Arjunan, Pandarasamy and Srivastava, Naman and Kumar, Kajeeth
             and Jati, Arindam and Ekambaram, Vijay and Dayama, Pankaj},
  journal = {ACM e-Energy},
  year    = {2026}
}
```

---
<!-- 
## Notice

EnergyFM builds on IBM Granite TSFM models available through the Hugging Face
`transformers` ecosystem. As the project evolves, code and documentation may
change accordingly. -->


