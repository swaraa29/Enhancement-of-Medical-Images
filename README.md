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

# Applications & Use Cases

This enhancement pipeline has potential impact in both clinical practice and medical AI development:

1. Clinical Diagnostics
Improves visibility of anatomical structures in low-quality MRI scans.
Aids radiologists in detecting brain abnormalities more accurately.
Reduces need for retakes due to low-quality imaging, saving time and cost.

2. Preprocessing for Medical AI Models
Enhances input data for downstream tasks like segmentation, classification, and tumor detection.
Reduces noise and artifacts that can confuse machine learning models.

3. Telemedicine & Remote Diagnostics
Enables clearer image transmission over bandwidth-limited networks.
Supports diagnosis in rural and low-resource healthcare settings where imaging quality is compromised.

4. Medical Education & Training
Produces clearer teaching images for student training and simulations.
Helps visualize subtle clinical signs more effectively.

5. Data Augmentation & Synthesis
Acts as a module in synthetic image pipelines to enhance realism in GAN-generated data for training AI models.

# Conclusion

In this project, we presented a robust medical image enhancement pipeline that combines the strengths of Generative Adversarial Networks (GANs) and Evolutionary Strategy (ES). By tuning generator hyperparameters such as filter size, kernel dimensions, and dropout rate through ES, we significantly improved model performance in enhancing brain MRI scans. Additionally, post-processing with CLAHE further refined image contrast while preserving structural features critical for diagnosis.

Quantitative evaluations using PSNR, SSIM, and L1 loss, along with visual assessments, confirm that the proposed method effectively enhances the diagnostic quality of medical images. The modular nature of this pipeline allows it to be adapted to other imaging modalities like CT, X-rays, and ultrasound.

This work contributes not only to the field of medical image processing but also serves as a foundational model for integrating biologically-inspired optimization techniques into deep learning pipelines for healthcare.



