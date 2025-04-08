# 🎨 sketch-colorizer-gan  
## Criminal Portrait Generation using GAN

This project explores the use of Generative Adversarial Networks (GANs) to generate realistic portraits of criminal suspects. It aims to automate and accelerate the process of forensic sketching through AI-generated images. The GAN was trained from scratch on a local machine using Jupyter Notebook, without using any pre-trained models.

---

## 🧠 Project Overview

Traditional forensic sketching is a time-intensive process that requires skilled artists and extensive interaction with witnesses. This project presents an alternative approach using a GAN-based model trained on facial datasets. The trained model takes in an input (conceptually, a sketch or feature vector) and generates a **single realistic portrait** that resembles a criminal suspect.

---

## 🧱 Features

- ✅ Fully custom GAN architecture
- ✅ Trained from scratch 
- ✅ Implemented and trained in Jupyter Notebook on local PC
- ✅ Produces a single output portrait per input
- ✅ Evaluated using Structural Similarity Index (SSIM)

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/sketch-colorizer-gan.git
cd sketch-colorizer-gan
```

### 2. Set Up the Environment

Ensure you have Python 3.8+ installed.

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
```

### 3. Prepare Dataset

- Download a facial image dataset such as CUHK or CelebA.
- Place images in the `data/` directory.
- Update paths in the notebook accordingly.

### 4. Train the Model

Open the notebook and begin training:

```bash
jupyter notebook notebooks/train_gan.ipynb
```

- The model was trained for **200 epochs** on local hardware.
- Training loss graphs for both generator and discriminator are visualized.

---

## 🖼️ Generate a Portrait

After training completes, the model can generate a **single realistic portrait**. Simply run the final generation cell in the notebook to produce an output stored in the `outputs/` directory.

---

## 🧪 Evaluation

The project evaluates generated portraits using:

- **Visual comparison**
- **Structural Similarity Index (SSIM)** — used to compare luminance, contrast, and structure with real images

A higher SSIM value (closer to 1) indicates greater similarity to real faces.

---

## 🛠 Requirements

- Python 3.8+
- Jupyter Notebook
- TensorFlow or PyTorch (based on your implementation)
- NumPy
- OpenCV or Pillow

Install everything via:

```bash
pip install -r requirements.txt
```

---

## 🌍 Applications

- Forensic criminal investigations
- Facial reconstruction for missing persons
- AI-generated face modeling

---

## ⚠️ Limitations & Future Work

- Currently supports **only one output** per input.
- More diverse datasets could improve output realism and generalizability.
- Future versions may include sketch-to-photo translation with more accurate control over facial features.
- Ethical considerations must be taken into account when applying generated portraits in law enforcement.

---

## 🙌 Acknowledgments

Inspired by advances in Generative Adversarial Networks (GANs) and real-world challenges in forensic sketching.

---
