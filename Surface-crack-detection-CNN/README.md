# Surface Crack Detection using CNN

AI-based binary image classification system that detects cracks on concrete/industrial surfaces using a Convolutional Neural Network (CNN) built with TensorFlow/Keras.

---

## 📌 Overview

Surface cracks are a key indicator of structural damage in buildings, bridges, and industrial infrastructure. Manual crack inspection is time-consuming and prone to human error. This project automates that process by training a CNN to classify surface images as **cracked (positive)** or **uncracked (negative)**, enabling faster and more consistent defect detection.

---

## 🧠 Approach

The pipeline follows a standard supervised image classification workflow:

1. **Data Loading** – Load labeled images from the `Positive/` and `Negative/` folders.
2. **Preprocessing** – Resize, normalize pixel values, and split into train/validation/test sets.
3. **Data Augmentation** – Apply random flips/rotations to improve generalization (if used).
4. **Model Building** – Construct a CNN architecture using TensorFlow/Keras (Conv2D, MaxPooling, Dense layers).
5. **Training** – Train the model on labeled images using binary cross-entropy loss.
6. **Evaluation** – Evaluate on a held-out test set using accuracy, precision/recall, and a confusion matrix.
7. **Prediction** – Run the trained model on new/unseen images to classify them.

---

## 🛠 Tech Stack

- **Language:** Python
- **Deep Learning:** TensorFlow, Keras
- **Image Processing:** OpenCV
- **Data Handling:** NumPy
- **Visualization:** Matplotlib
- **Evaluation:** Scikit-learn

---

## 📂 Dataset

- **Source:** [Surface Crack Detection Dataset – Kaggle](https://www.kaggle.com/datasets/arunrk7/surface-crack-detection)
- **Classes:** `Positive` (crack present), `Negative` (no crack)
- **Image size:** 227 x 227 px, RGB
- **Total images:** *(fill in — e.g., 40,000: 20,000 per class)*

## 📁 Project Structure

```
surface-crack-detection-cnn/
│
├── train.py              # Model training script
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation 
│
└── dataset/
    ├── Positive/
    └── Negative/
```
---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/Rukmini-Gaikwad/Surface-Crack-Detection-CNN.git
cd Surface-Crack-Detection-CNN

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download the dataset from Kaggle and place it in the dataset/ folder
#    (see Dataset section above)

# 4. Train the model
python train.py
```

---

## 🔮 Future Improvements

- Experiment with transfer learning (e.g., MobileNetV2, ResNet) to compare against the custom CNN
- Add Grad-CAM visualization to highlight which regions of the image influenced the crack prediction
- Deploy the trained model as a simple Streamlit app for live image upload and prediction
- Extend to multi-class defect detection (e.g., cracks vs. spalling vs. corrosion)

---
