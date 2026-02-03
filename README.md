# Batik Image Classification using a Convolutional Neural Network

## Overview
This project explores **image classification of Indonesian batik motifs** using a **convolutional neural network (CNN) trained from scratch**. Batik is a culturally significant textile with region-specific patterns, making it a challenging and meaningful real-world classification problem.

The objective of this project is to build and evaluate a CNN capable of predicting the **region of origin** of a batik image across **20 different batik classes**.

---

## Dataset
- Source: Kaggle (https://www.kaggle.com/datasets/hendryhb/batik-nusantara-batik-indonesia-dataset)
- Total classes: 20 batik motifs
- Images organized by class folders
- Separate training and testing sets
- Relatively small dataset, suitable for exploring CNN fundamentals

---

## Methodology
The project follows a standard deep learning workflow:
1. Data preprocessing (image resizing and normalization)
2. Data augmentation to reduce overfitting
3. CNN architecture design (three convolutional blocks)
4. Model training using Adam optimizer and categorical crossentropy loss
5. Evaluation using accuracy, loss, and a confusion matrix

---

## Results
- Test accuracy: ~32%
- Test loss: ~2.32
- Training and validation curves indicate underfitting
- Confusion matrix reveals frequent misclassification between visually similar batik patterns

These results highlight the limitations of training a CNN from scratch on a small, fine-grained image dataset.

---

## Key Takeaways
- CNNs can learn meaningful features from batik patterns but struggle with limited data
- Visual similarity between classes significantly affects performance
- Transfer learning is a natural next step for improving results

---

## Future Work
- Apply transfer learning using pretrained CNNs (e.g. MobileNetV2)
- Train on a larger batik dataset
- Compare baseline CNN with pretrained models

---

## Full Report
A detailed analysis of the model architecture, training process, evaluation, and limitations is provided in the accompanying project report.

---

## Files in This Repository
- `batik_cnn_from_scratch.ipynb` – Google Colab notebook containing the full implementation
- `Batik_CNN_Report.pdf` – Full project report
- `README.md` – Project overview
