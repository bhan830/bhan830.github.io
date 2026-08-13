---
title: WiseSpine
subtitle: Deep Learning Pipeline for Automated Cobb Angle Measurement
summary: "Data preparation outperforms architecture selection in automated scoliosis assessment."
featured_image: ''
tags:
  - Python
  - PyTorch
  - Medical Imaging
  - Segmentation
  - Data-Centric AI
  - AWS
date: 2025-11-01
institution: University of Washington | Seattle, WA
affiliation: Amazon Web Services (AWS), UW Harborview Medical Center
start_date: 2025-11-01
end_date: ''
---

WiseSpine is a data-centric AI pipeline for automated Cobb angle measurement from spine X-rays, demonstrating that data preparation choices, rather than model architecture, are the primary driver of clinical measurement accuracy. Using the AASCE MICCAI 2019 dataset of 481 AP spinal X-rays, the project converts sparse vertebral landmark annotations into dense segmentation ground truth and evaluates how those upstream decisions propagate to a clinical endpoint.

## Key Contributions

- Engineered a landmark-to-mask conversion pipeline transforming sparse 4-corner vertebral annotations into dense segmentation ground truth via quadrilateral construction and watershed boundary refinement, reducing Cobb angle MAE by up to 4.36° (30.1%).
- Conducted a controlled 2×4 factorial ablation across three architectures (nnU-Net 2D, Attention U-Net, UNet++) and two data conditions on 481 AP spinal X-rays, finding data preprocessing improvements were 2–4× larger than those from architecture switching alone.
- Empirically tuned watershed distance threshold (14.6 px) via validation sweep, exposing that ±2 px variations propagate to clinically meaningful Cobb angle differences invisible to standard Dice metrics.
- Collaborated with AWS engineers on scalable AI infrastructure design for medical imaging workloads.

## Technologies

**Languages:** Python

**AI & Machine Learning:** PyTorch, Segmentation (nnU-Net 2D, Attention U-Net, UNet++), Watershed Segmentation, Data-Centric AI

**Data & Evaluation:** Landmark-to-Mask Conversion, Ablation Studies, Cobb Angle Estimation, Regional & Severity Analysis

**Infrastructure:** Amazon Web Services (AWS), Medical Imaging Pipelines
