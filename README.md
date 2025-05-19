# 🧠 Decoding Emotional Brain Activity Patterns from fMRI: SVM vs. GCN

This project presents a comparative study of **Support Vector Machines (SVM)** and **Graph Convolutional Networks (GCN)** for decoding emotional states—**fear** vs. **neutral**—from fMRI data using the Human Connectome Project (HCP) Emotion dataset.

## 📌 Overview

The goal of this study is to evaluate the performance and interpretability of traditional and graph-based machine learning models in decoding neural activity patterns. We focus on binary classification of emotional states from functional MRI signals and explore the challenges and opportunities presented by structured neuroimaging data.

## 🧬 Dataset

- **Source**: Human Connectome Project (HCP) - Emotion Task
- **Subjects**: 340 participants
- **Features**: BOLD activity from 360 brain regions during fear and neutral stimuli across two runs
- **Labels**: Binary emotion state (Fear / Neutral)

## 🔍 Methodology

- **Data Split**: 80% training, 20% testing (subject-wise)
- **Models**:
  - **SVM** for baseline tabular classification
  - **GCN** (2-layer, 4-layer, 6-layer variants) to leverage graph structures in brain connectivity

- **Evaluation Metric**: Accuracy, Precision, Recall, F1-score

## 🧪 Results

| Metric      | SVM     | GCN     |
|-------------|---------|---------|
| Accuracy    | 56.93%  | 77.57%  |
| Precision   | 62.97%  | 79.08%  |
| Recall      | 34.43%  | 77.57%  |
| F1 Score    | 44.52%  | 77.28%  |

- GCN significantly outperformed SVM across all evaluation metrics, highlighting its ability to model spatial dependencies in brain data.

## ⚙️ Tools & Libraries

- Python
- Scikit-learn (SVM)
- PyTorch Geometric / DGL (for GCNs)
- Google Colab (for training)
- HCP Dataset

## 🌍 Applications

- Mental health diagnostics
- Affective computing
- Emotion-aware human-computer interaction
- Cognitive neuroscience research

## ⚠️ Limitations

- No preprocessing (e.g., normalization, filtering) applied, which may affect model robustness.
- GCN training limited by computational resources (batch size = 1).

## 📖 References

- Rastegarnia et al., *Brain decoding of the Human Connectome Project tasks in a dense individual fMRI dataset* (NeuroImage, 2023)
- Zhang et al., *Deep learning models of cognitive processes constrained by human brain connectomes* (Medical Image Analysis, 2022)

## 🤝 Acknowledgements

- **Hadi Motamedi**  
- **Sanjeev Nara**

## 👨‍👩‍👧‍👦 Team Neuronauts
Mohammad Elsherif
Amirmahdi Manzari Tavakoli 
Farhan Ali
Amirhossein Sadr
---
