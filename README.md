**Overview:**

This project detects industrial surface cracks using Convolutional Neural Networks (CNN).
The model is trained on crack and non-crack surface images to automatically classify damaged surfaces.

The project performs:

Image preprocessing
Data augmentation
CNN model training
Model evaluation
Surface crack prediction

Technologies Used

Python
TensorFlow / Keras
NumPy
Matplotlib
Scikit-lear

Project Structure:

surface-crack-detection-cnn/
│
├── train.py            # Model training code
├── requirements.txt    # Required libraries
├── README.md           # Project documentation
│
└── dataset/
    │
    ├── Positive/       # Crack images
    └── Negative/       # Non-crack images

**Dataset**

Dataset used for this project:

https://www.kaggle.com/datasets/arunrk7/surface-crack-detection

This dataset contains positive and negative surface crack images used for training and evaluating the CNN model for industrial crack detection.
