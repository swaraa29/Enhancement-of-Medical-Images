# Enhancement-of-Medical-Images
# Enhancing Medical Image Quality Using GANs with Evolutionary Hyperparameter Optimization

This repository presents a deep learning-based pipeline to enhance low-quality medical brain MRI images using a U-Net-based Generative Adversarial Network (GAN), optimized via Evolutionary Strategy. The goal is to improve image clarity and structural fidelity for better diagnostic interpretation.

# Overview

Medical images often suffer from low contrast, noise, and poor resolution. This project integrates:

- A **Pix2Pix GAN** with U-Net generator and PatchGAN discriminator
- **Evolutionary Strategy (ES)** to optimize key hyperparameters
- **CLAHE** (Contrast Limited Adaptive Histogram Equalization) for post-processing
- Quantitative evaluation using **PSNR**, **SSIM**, and **L1 Loss**

# Key Contributions

- Developed a GAN-based enhancement pipeline tailored for brain MRI scans.
- Applied Evolutionary Strategy for automated tuning of:
  - Number of filters
  - Kernel size
  - Dropout probability
- Combined GAN outputs with CLAHE for local contrast improvement.
- Achieved consistent improvement in PSNR and SSIM scores.


