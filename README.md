# Audio Denoiser

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![Python](https://img.shields.io/badge/Python-3.8+-green)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red)
![Librosa](https://img.shields.io/badge/Librosa-0.10-blue)

A hybrid **audio denoising** project using **Wave-U-Net with ASPP** and classical filters (**MMSE-LSA**, **Wiener**) to enhance noisy speech.

---

## Features

**Deep Learning Based**
- Wave-U-Net with Atrous Spatial Pyramid Pooling (ASPP)
- Encoder–Decoder with skip connections capturing multi-scale temporal features
- Trainable on waveform or spectrogram input

**Classical Signal Processing**
- Wiener filtering with estimated noise PSD
- MMSE-LSA with decision-directed SNR estimation
- Residual noise suppression

**Evaluation**
- Objective metrics: **SNR**, **PSNR**, **SSIM**
- Visualizations: waveforms & spectrograms

---

## Installation

### Prerequisites
- Python 3.8+
- PyTorch
- Librosa, NumPy, SciPy, Matplotlib, scikit-image

  ```bash
  # Clone the repository
  git clone https://github.com/AadharshRamachandran/audiodenoiser.git
  cd audiodenoiser
  pip install -r requirements.txt


**Launch Notebooks**

Deep Learning Approach.ipynb — train and evaluate Wave-U-Net + ASPP

Traditional Approach.ipynb — experiment with MMSE-LSA and Wiener filtering

**Project Structure**

audiodenoiser/

├── Deep Learning Approach.ipynb      # Train/evaluate Wave-U-Net + ASPP

├── Traditional Approach.ipynb        # MMSE-LSA & Wiener filter experiments

├── requirements.txt                  # Python dependencies

├── README.md                         # Project overview (this file)

Outputs can be seen in this link
Link 1 : https://www.kaggle.com/code/aadharshramachandran/signals-and-systems-objective-1/output
Link 2 : https://www.kaggle.com/code/aadharshramachandran/signals-and-systems-objective-2/output
