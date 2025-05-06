# Liver Tumor Segmentation with Super-Resolution and Attention Mechanisms

This repository contains the complete code for the project **"Liver Tumor Segmentation with Super-Resolution and Attention Mechanisms"**, developed as part of CS437 (Advanced Machine Learning). The project introduces a multi-stage deep learning pipeline that segments liver tumors in CT scans and generates diagnostic reports using GPT-4.

## Project Overview

The pipeline is composed of the following stages:

1. **Liver Segmentation**  
   A U-Net with a ResNet34 backbone performs binary liver segmentation on 2D CT slices.

2. **Super-Resolution Enhancement**  
   FSRCNN is used to upscale liver-region patches to highlight small, low-contrast tumors.

3. **Tumor Segmentation**  
   A custom Deep Attention U-Net (v1.2) segments tumors from super-resolved liver patches.

4. **Diagnostic Report Generation**  
   Extracted tumor metadata (count, size, location) is fed into GPT-4 to generate concise radiology-style summaries.

---

## Files

- `Group21_Final_Project.ipynb`:  
  The main notebook. Includes everything from data loading and preprocessing to model training, inference, and GPT-based report generation.

---

## Dataset

We use the [LiTS Dataset](https://competitions.codalab.org/competitions/17094) (Liver Tumor Segmentation Challenge), which includes 131 CT volumes with annotated liver and tumor masks.

**Note:** The dataset is not included in this repository. Please register and download it from the official challenge page.

---

