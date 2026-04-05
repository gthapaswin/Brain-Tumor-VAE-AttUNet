#Brain Tumor Segmentation using VAE + Attention U-Net

## Overview
This project implements a **hybrid deep learning model** combining:
- Variational Autoencoder (VAE)
- Attention U-Net

The goal is to improve **brain tumor segmentation from MRI scans** by leveraging both **generative and discriminative learning**.

---

## Objective
- Perform accurate tumor segmentation
- Improve feature learning using VAE
- Compare hybrid model with baseline Attention U-Net

---

## Model Architecture

### 🔹 Pipeline 
MRI Image → VAE (Reconstruction & Feature Learning) → Attention U-Net → Segmentation Mask


---

## Models Used

| Model | Purpose |
|------|--------|
| Attention U-Net | Baseline segmentation |
| VAE | Feature extraction & denoising |
| VAE + Attention U-Net | Proposed hybrid model |

---

## 📊 Evaluation Metrics

- Dice Score
- IoU (Intersection over Union)
- Precision
- Recall
- F1 Score
- ROC Curve (AUC)

---

## 📈 Results

| Metric | Value |
|-------|------|
| Dice Score (Baseline) | 0.378 |
| Dice Score (Proposed) | 0.397 |
| IoU | 0.249 |
| Precision | 0.062 |
| Recall | 0.678 |
| F1 Score | 0.113 |
| AUC | 0.618 |

---

## Dataset

- Brain Tumor MRI Dataset  : https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset
- Brain Tumor Classification Dataset  : https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri

Folder structure:
DL/
├── Training/
├── Testing/

DL-segmentation/
├── Training/
├── Testing/


---

## Tech Stack

- Python
- PyTorch
- Google Colab
- NumPy
- Matplotlib
- Scikit-learn

---

## How to Run

1. Open the notebook in Google Colab  
2. Mount Google Drive  
3. Update dataset paths if needed  
4. Run all cells  

---

## Key Insight

The hybrid VAE + Attention U-Net model improves segmentation performance by:
- Learning better latent representations  
- Reducing noise in MRI images  
- Enhancing tumor region detection  

---

## Conclusion

The proposed hybrid model demonstrates that **generative pretraining (VAE)** can enhance **segmentation performance**, although further optimization is required to improve precision.
