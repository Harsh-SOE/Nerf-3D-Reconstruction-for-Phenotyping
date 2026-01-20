# 🌱 Plant Phenotyping using Neural Radiance Fields (NeRF)

This repository contains an experimental implementation of **Plant Phenotyping using Neural Radiance Fields (NeRF)**. The project focuses on reconstructing high‑quality **3D representations of plants from multiple 2D images**, enabling improved analysis of plant structure and growth traits.

---

## 📌 Motivation

Plant phenotyping is essential in agriculture and plant science for:

* Growth monitoring
* Structural analysis
* Trait extraction (height, leaf area, geometry)
* Stress and health assessment

Traditional 2D imaging fails to capture spatial geometry accurately. **Neural Radiance Fields (NeRF)** provide a powerful alternative by learning a **continuous 3D scene representation** from sparse multi‑view images.

This project explores how NeRF can be applied to plant phenotyping tasks.

---

## 🧠 What is NeRF?

NeRF (Neural Radiance Fields) represents a scene as a function:

```
F(x, y, z, θ, φ) → (RGB, Density)
```

A neural network learns to map 3D spatial coordinates and viewing directions to:

* Color (RGB)
* Volume density

Using **volume rendering**, novel views of the scene can be synthesized with high fidelity.

---

## 📘 Notebook Overview

The notebook covers the following steps:

1. Understanding the NeRF pipeline
2. Loading and preprocessing multi‑view images
3. Ray generation from camera poses
4. Positional encoding
5. NeRF network architecture
6. Volume rendering equation
7. Training loop
8. Rendering novel views
9. Visualization of results

The implementation is intended for **learning and experimentation**, not optimized for production.

---

## 📂 Repository Structure

```
plant-phenotyping-nerf/
│
├── plant-phenotyping-nerf.ipynb   # Main notebook
├── README.md                      # Project documentation
├── requirements.txt               # Python dependencies
└── .gitignore                     # Ignored files
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/plant-phenotyping-nerf.git
cd plant-phenotyping-nerf
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate   # Linux / macOS
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
plant-phenotyping-nerf.ipynb
```

A GPU is strongly recommended for training.

---

## 🧪 Requirements

* Python 3.9 or later
* PyTorch
* NumPy
* OpenCV
* Matplotlib
* Jupyter Notebook

Detailed dependencies are listed in `requirements.txt`.

---

## 🖥️ Hardware Recommendations

* **GPU**: NVIDIA GPU with CUDA support
* **RAM**: 8 GB minimum (16 GB recommended)
* **CPU**: Multi‑core processor

NeRF training is computationally intensive.

---

## 🚀 Possible Extensions

* Train on real plant phenotyping datasets
* Use Instant‑NGP for faster training
* Convert NeRF output to mesh (NeRF → Mesh)
* Extract phenotypic traits from 3D geometry
* Temporal plant growth modeling (4D NeRF)
* Integrate semantic segmentation

---

## 📊 Applications

* Agricultural research
* Crop monitoring
* Precision farming
* Plant morphology analysis
* 3D computer vision research

---

## 📚 References

* Mildenhall et al., *NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis*, ECCV 2020
* NeRF official project page
* Recent research on 3D plant phenotyping

---

## ⚠️ Disclaimer

This project is intended for **educational and research purposes only**. It is not optimized for large‑scale or real‑time phenotyping systems.

---

## ✍️ Author

**Harsh Vardhan Yadav**
Computer Science Student
Interests: Computer Vision, Deep Learning, 3D Reconstruction

---

## ⭐ Acknowledgements

* NeRF research community
* PyTorch ecosystem
* Open‑source contributors

---

If you find this project useful, consider giving it a ⭐ on GitHub.
