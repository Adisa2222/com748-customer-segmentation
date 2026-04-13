# com748-customer-segmentation
Code for MSc Research Project: A comparative evaluation of CTGAN, bootstrapping, and Gaussian noise for customer segmentation under data scarcity

# Customer Segmentation Under Data Scarcity: CTGAN vs. Simpler Augmentation Methods

This repository contains the implementation for the MSc Computer Science research project at Ulster University (COM748).

## Overview
- Compares **CTGAN**, **bootstrapping**, and **Gaussian noise** for synthetic data augmentation
- Evaluates performance on the Mall Customers dataset (n=200)
- Metrics: cluster stability (Jaccard), interpretability (% match to retail archetypes), distributional fidelity (Wasserstein, chi-square)

## Files
- `02_augmentation_and_evaluation.ipynb`: Full implementation, results, and visualisations

## Requirements
- Python 3.10+
- Dependencies listed in `requirements.txt` (if provided)

## Dataset
- Uses the publicly available **Mall Customers dataset** (n=200), commonly used in clustering tutorials.
- Source: https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python  
  *(Note: Dataset not included in this repo due to redistribution restrictions)*

## Reproducibility
- All random seeds fixed (`np.random.seed(42)`)
- Results match those reported in the thesis:  
  - CTGAN interpretability: 6.8%  
  - CTGAN stability: 0.196  
  - Wasserstein distance (Income): 12.41

## Author
Oluwadolapo Nasirudeen Adisa  
MSc Computer Science, Ulster University  
Student ID: B01001103
