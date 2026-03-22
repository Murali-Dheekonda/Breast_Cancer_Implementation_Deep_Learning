# Breast_Cancer_Implementation_Deep_Learning
Comparative analysis of deep learning models for histopathological breast cancer classification using BreaKHis dataset with preprocessing, class imbalance handling, and evaluation metrics.


# 🧬 Breast Cancer Histopathology Image Classification

## 📌 Overview

This project presents a deep learning-based system for classifying breast cancer histopathology images into **benign** and **malignant** categories. The goal is to assist in early and accurate diagnosis by automating medical image analysis using computer vision techniques.

Manual examination of histopathological slides is time-consuming and subject to human variability. This project addresses these challenges by implementing and comparing multiple deep learning architectures.

---

## 📊 Dataset

* **Dataset**: BreaKHis 400X Histopathology Dataset
* **Total Images**: 1,693

  * Benign: 547
  * Malignant: 1,146
* **Split**:

  * Training: 80%
  * Validation: 20%

### 🔧 Preprocessing Steps

* Image resizing to **128x128 pixels**
* Normalization (pixel values scaled between 0–1)
* Data augmentation:

  * Rotation
  * Zoom
  * Horizontal flipping
* Class imbalance handling using **class weights**

---

## 🧠 Models Implemented

The project evaluates the performance of multiple deep learning architectures:

* **CNN (Custom Model)**
* **ResNet50 (Transfer Learning)**
* **EfficientNetB0 (ViT-style approach)**
* **MobileNetV2**

---

## ⚙️ Implementation Details

* **Framework**: TensorFlow / Keras
* **Language**: Python
* **Batch Size**: 64
* **Epochs**: 5
* **Optimizer**: Adam (learning rate = 0.0001)
* **Loss Function**: Binary Cross-Entropy

---

## 📈 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC Curve & AUC Score

---

## 📊 Results

| Model        | Accuracy   |
| ------------ | ---------- |
| CNN          | **86.14%** |
| EfficientNet | 67.55%     |
| MobileNetV2  | 52.51%     |
| ResNet50     | 37.17%     |

### 🔍 Key Findings

* CNN outperformed all other models despite being simpler.
* Complex models like ResNet50 underperformed due to limited dataset size.
* Class imbalance significantly affected model predictions.
* Preprocessing and augmentation improved generalization.

---

## 📷 Visual Outputs

* Sample histopathology images
* Data distribution plots
* Model architecture diagrams
* Confusion matrices
* ROC curves

---

## 🧪 Ablation Study

* Removing class weights led to strong bias toward the majority class.
* Removing data augmentation caused overfitting.
* Preprocessing steps were critical for stable performance.

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📁 Project Structure

```
├── notebooks/
│   └── Breast_Cancer_Implementation_Deep_Learning.ipynb
├── report/
│   └── Breast Cancer Histopathology Image Classification.docx
├── README.md
```

---

## 🚀 How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/Breast_Cancer_Implementation_Deep_Learning.git
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Run the Jupyter Notebook:

```
jupyter notebook
```

---

## 🔮 Future Improvements

* Train on larger datasets for better generalization
* Hyperparameter tuning
* Ensemble learning models
* Integration into real-time clinical systems

---

## 📌 Conclusion

This project demonstrates that deep learning can significantly improve breast cancer diagnosis through automated image classification. Simpler architectures like CNN can outperform complex models when working with smaller datasets, emphasizing the importance of proper model selection and preprocessing.

---

## 👤 Author

**Murali Dheekonda**
MSc Data Science Student | Aspiring Data Analyst

---

## ⭐ If you found this useful

Give this repository a ⭐ and share your feedback!
