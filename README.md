
```markdown
# 👁️ Automated Retinal Cyst Detection in OCT Images

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-orange)
![Medical Imaging](https://img.shields.io/badge/Domain-Medical%20Imaging-red)
![Status](https://img.shields.io/badge/Project-MSc%20Research-success)

> Lightweight and interpretable retinal cyst segmentation system using classical image processing techniques on Optical Coherence Tomography (OCT) scans.

---

## 📌 Overview

Retinal cysts are key biomarkers in diseases such as Diabetic Macular Edema (DME) and Age-related Macular Degeneration (AMD). Manual segmentation is slow and subjective.

This project builds an automated segmentation pipeline using **classical computer vision** instead of deep learning — prioritizing transparency, efficiency, and reproducibility.

The system performs:
- Image preprocessing
- Adaptive threshold-based segmentation
- Morphological refinement
- Quantitative evaluation using Dice & IoU metrics

---

## 🚀 Key Features

- Classical CV-based medical segmentation
- No GPU or large datasets required
- Adaptive thresholding for cyst detection
- CLAHE contrast enhancement
- Speckle noise reduction
- Morphological post-processing
- Quantitative & visual evaluation
- Lightweight research-grade pipeline

---

## 🏗️ Pipeline

```

OCT Image
↓
CLAHE Contrast Enhancement
↓
Median Noise Filtering
↓
Adaptive Threshold Segmentation
↓
Morphological Refinement
↓
Cyst Mask Output + Metrics

```

---

## 🔬 Methodology

### Preprocessing
- CLAHE contrast enhancement
- Median filtering for speckle noise

### Segmentation
- Local adaptive thresholding
- 35×35 window size
- Offset value: 10

### Post-Processing
- Morphological opening
- Small object removal
- Hole filling

---

## 📊 Evaluation Metrics

- Dice Coefficient
- Intersection over Union (IoU)

**Average Dice:** 0.179  
**Average IoU:** 0.100

---

## 📈 Results

| Metric | Score |
|-------|------|
| Dice | 0.179 |
| IoU | 0.100 |

Large cysts were detected effectively, while small low-contrast regions remain challenging — providing a strong baseline for future hybrid or deep learning methods.

---

## 🧰 Tech Stack

- Python
- OpenCV
- scikit-image
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📁 Project Structure

```

retinal-cyst-segmentation/
│
├── data/
│   ├── images/
│   └── masks/
│
├── notebooks/
│   └── segmentation.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── segmentation.py
│   ├── postprocessing.py
│   └── evaluation.py
│
├── results/
├── requirements.txt
└── README.md

````

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/retinal-cyst-segmentation.git
cd retinal-cyst-segmentation
pip install -r requirements.txt
````

---

## ▶️ Usage

Run notebook:

```bash
jupyter notebook
```

Or execute pipeline:

```bash
python main.py
```

---

## 💡 Engineering Highlights

* Fully interpretable medical AI pipeline
* Lightweight classical CV implementation
* Modular segmentation workflow
* Reproducible experiments
* No deep learning dependency

---

## 🔮 Future Work

* Hybrid classical + deep learning segmentation
* U-Net comparison
* Clinical dashboard interface
* API deployment (FastAPI)
* Explainable AI integration

---

## 👨‍🎓 Author

**Vivan Kushal Heneger**
MSc Data Science — Newcastle University
📧 [v.k.heneger2@newcastle.ac.uk](mailto:v.k.heneger2@newcastle.ac.uk)

---

## 📜 License

Academic & research use only.


```
