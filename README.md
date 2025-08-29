
# MVTec-AD Anomaly Detection with Anomalib

This repository applies anomaly detection to the [MVTec Anomaly Detection (MVTec-AD)](https://www.mvtec.com/company/research/datasets/mvtec-ad) dataset using the [Anomalib](https://github.com/openvinotoolkit/anomalib) library.  
We experiment with three state-of-the-art models — **PatchCore**, **FastFlow**, and **STFPM** — and evaluate their performance on pixel-level and image-level tasks.

---

## 📌 Project Overview
- **Dataset:** [MVTec-AD](https://www.mvtec.com/company/research/datasets/mvtec-ad) (industrial inspection dataset with 15 object & texture categories).  
- **Focus categories:** Tile, Leather, Grid (flat surface defects).  
- **Models used:** PatchCore, FastFlow, STFPM.  
- **Evaluation metrics:** AUROC & F1-Score (pixel-level and image-level).  
- **Environment:** Python, PyTorch, Anomalib 2.0.0.dev0, Jupyter Notebook.  

---

## 🚀 Features
- End-to-end anomaly detection pipeline using Anomalib.  
- Training and evaluation of three benchmark models.  
- Pixel- and image-level AUROC/F1 reporting.  
- Tutorial-style Jupyter Notebook with code, plots, and results.  
- Reproducible workflows designed for easy extension to other categories.  

---

## 📊 Results

Overall performance across the dataset:

| Metric          | PatchCore | FastFlow | STFPM |
|-----------------|:---------:|:--------:|:-----:|
| **Pixel AUROC** | **0.981** |  0.969   | 0.929 |
| **Pixel F1**    | **0.730** |  0.000   | 0.000 |
| **Image AUROC** | **1.000** | **1.000**| 0.982 |
| **Image F1**    | **0.992** | **0.992**| 0.960 |

> 📌 Note: These are **overall AUROC/F1 values**. Per-category results (e.g., *tile, leather, grid*) can be added once logged.  

---

## ⚙️ Setup

1. **Clone this repository**
   ```bash
   git clone https://github.com/<your-username>/mvtec-ad-anomaly-detection.git
   cd mvtec-ad-anomaly-detection
````

2. **Create environment & install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Download MVTec-AD dataset**
   [MVTec-AD download](https://www.mvtec.com/company/research/datasets/mvtec-ad)
   Place it under:

   ```
   ./datasets/mvtec
   ```

---

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook mvtec-ad-anomaly-detection-with-anomalib-library.ipynb
```

The notebook contains:

* Model training & inference
* AUROC/F1 evaluation
* Visualizations of anomaly heatmaps and metrics

---

## 📚 References

* [MVTec-AD Dataset](https://www.mvtec.com/company/research/datasets/mvtec-ad)
* [Anomalib Library](https://github.com/openvinotoolkit/anomalib)

---

## ✨ Acknowledgements

This project was developed as part of anomaly detection research on industrial inspection datasets.
Special thanks to the maintainers of **Anomalib** for providing an excellent framework for anomaly detection.

---

```
