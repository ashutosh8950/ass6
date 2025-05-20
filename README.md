# DeepFake Image Detection with CNNs, Transformers & Ensemble Approaches

This repository contains the LaTeX source and supporting materials for a research project focused on detecting DeepFake facial images using a combination of pre-trained Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs). The work evaluates model efficiency and explores ensemble strategies in low-data environments.

---

## 📖 Project Summary

With the rise of AI-generated content, DeepFakes have become a major challenge in verifying digital authenticity. This project aims to classify face images as real or fake using a small subset of the FaceForensics++ dataset. It compares different deep learning models and examines how combining models can improve reliability.

---

## 🔍 Models Evaluated

- **VGG16** – Classic CNN model for baseline
- **ViT** – Vision Transformer architecture
- **GenConViT** – CNN + Transformer hybrid
- **DeepFake-Adapter** – Fine-tuned detector for DeepFake tasks

---

## ⚙️ Experimental Setup

- **Dataset**: 200 images (100 real, 100 fake) from FaceForensics++
- **Image Dimensions**: 128x128 pixels
- **Preprocessing Steps**:
  - Image normalization
  - Light augmentation techniques
- **Training Configuration**:
  - Loss Function: Binary Cross-Entropy
  - Optimizer: Adam
  - Early stopping applied for efficient training
- **Metrics Used**:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
- **Ensemble Method**:
  - Soft voting to combine predictions from different models

---

## 📈 Key Outcomes

- **Top Accuracy**: 70% with VGG16
- **ViT** struggled due to the dataset size
- **Ensemble Models** showed slight gains in prediction consistency

---

## 📂 Folder Layout

├── images/ # Visuals and diagrams
│ ├── vgg16_architecture.png
│ ├── vit_architecture.png
│ ├── genconvit_architecture.png
│ ├── deepfake_adapter_architecture.png
│ ├── sample_faces.png
│ ├── confusion_cnn.png
│ ├── confusion_vit.png
│ ├── accuracy_bar.png
│ └── metric_comparison.png
│
├── DeepFake_Detection.tex # Main LaTeX document
├── README.md # Project documentation
└── references.bib # Citation file (if separated)

---

## 📦 Requirements

To compile the LaTeX file, ensure your setup includes these packages:

- `graphicx`
- `amsmath`
- `cite`
- `caption`
- `multirow`
- `booktabs`
- `hyperref`
- `placeins` (recommended)

You can use a full LaTeX distribution like **TeX Live** or **MiKTeX**, or compile online using **Overleaf**.

---

## 📚 Citation Sources

This work references the following:

- FaceForensics++ Dataset
- Research papers on VGGNet and Vision Transformers
- Hugging Face Transformers Library
- Scikit-learn for metrics and evaluation

Refer to the `.bib` file or LaTeX source for complete citation details.

---

## 👨‍💻 Contributor

**Ashutosh Gupta**  
Roll Number: 102203230
📧 Email: guptaashutosh8950@gmail.com  
🏫 Thapar Institute of Engineering and Technology

---

## 🚧 Scope for Enhancement

- Add support for audio-visual multimodal detection
- Test hybrid models on larger and more diverse datasets
- Use explainability tools like Grad-CAM to visualize model focus areas

---

## 📜 License

This project is intended for academic and research usage. You are free to use or modify the materials with appropriate attribution to the original authors.
