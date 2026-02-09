# 🧬 GNN Protein Function Prediction

> Multi-relational Link Prediction using Variational Graph Autoencoder (VGAE)

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org)
[![Colab](https://img.shields.io/badge/Google-Colab-yellow.svg)](https://colab.google)

## 📋 Đồ Án

**Môn học:** IS353 - Mạng Xã Hội  
**Đề tài:** Graph Neural Networks in Predicting Protein Function and Interactions  
**Model:** VGAE (Variational Graph Autoencoder)  
**Dataset:** BioSNAP-Polypharmacy

## 🎯 Mục Tiêu

Dự đoán tác dụng phụ khi sử dụng nhiều loại thuốc cùng lúc (polypharmacy side effects) bằng cách:
- Mô hình hóa mạng lưới thuốc-thuốc dưới dạng đồ thị đa quan hệ
- Sử dụng VGAE với R-GCN Encoder để học biểu diễn node
- Dự đoán liên kết mới với DistMult Decoder

## 🏗️ Kiến Trúc

```
Input Graph → R-GCN Encoder → Latent Space Z → DistMult Decoder → Link Predictions
```

## 📁 Cấu Trúc

```
├── notebooks/           # Jupyter notebooks
│   ├── 01_data_exploration.ipynb
│   ├── 02_model_implementation.ipynb
│   ├── 03_training.ipynb
│   ├── 04_grid_search.ipynb
│   └── 05_evaluation.ipynb
├── figures/             # Hình ảnh visualization
├── models/              # Model checkpoints
├── reports/             # Báo cáo Word + Slides
├── data/                # Dataset
└── README.md
```

## 🚀 Quick Start

```bash
# Clone repo
git clone https://github.com/<username>/gnn-protein-prediction.git

# Mở trên Google Colab
# Upload notebooks/ lên Colab và chạy theo thứ tự 01 → 05
```

## 📊 Dataset

**BioSNAP-Polypharmacy** từ Stanford:
- ~600 drugs
- ~900+ loại tác dụng phụ (relation types)
- ~4.5M drug-drug interactions

## 📈 Kết Quả

| Metric | Score |
|--------|-------|
| ROC-AUC | TBD |
| PR-AUC | TBD |

## 📚 References

1. Kipf & Welling - "Variational Graph Autoencoders" (2016)
2. Zitnik et al. - "Modeling polypharmacy side effects with GNNs" (2018)
3. Schlichtkrull et al. - "Modeling Relational Data with R-GCN" (2018)

## 👤 Author

- Student ID: [Your ID]
- University: UIT
