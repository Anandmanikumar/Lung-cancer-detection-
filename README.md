Lung Cancer Detection Using CNN

A deep learning project using Convolutional Neural Networks (CNN) for early lung 
disease detection (Normal vs Pneumonia chest X-rays). This project applies image 
preprocessing, data augmentation, and CNN-based classification to assist doctors in diagnosis.

 Project Overview

Built and trained a CNN model for detecting lung diseases from chest X-rays.

Dataset used: Chest X-ray Pneumonia Dataset (Kaggle).

Achieved 85–90% accuracy on validation/test sets.

Implemented preprocessing, augmentation, and evaluation inside the notebook.

 Repository Structure
LungCancerDetection-CNN/
│── Lung_Cancer_Detection_CNN.ipynb   # Main Jupyter Notebook
│── requirements.txt                   # Python dependencies
│── README.md                          # Project documentation
│── results/                           # (Optional) Plots, saved metrics

Dataset

Source: Chest X-ray Pneumonia Dataset (Kaggle)

Classes:

NORMAL → Healthy lungs

PNEUMONIA → Diseased lungs

Preprocessing:

Resized images to 256×256

Normalized pixel values to [0,1]

Applied data augmentation (rotation, zoom, flip, shift)

 Model Architecture

Input: 256×256 grayscale X-ray

CNN with 5 convolutional blocks + dense layers

Optimizer: RMSprop

Loss: Binary Crossentropy

Metric: Accuracy

 How to Run
1. Clone Repository
git clone https://github.com/Anandmanikumar/Lung-cancer-detection-

2. Install Dependencies
pip install -r requirements.txt

3. Download Dataset

Download dataset from Kaggle
.

Place dataset inside data/ folder in the same structure:

data/
│── train/
│   ├── NORMAL/
│   └── PNEUMONIA/
│── val/
│   ├── NORMAL/
│   └── PNEUMONIA/
│── test/
│   ├── NORMAL/
│   └── PNEUMONIA/

4. Open Notebook
jupyter notebook lung-cancer-detection.ipynb


Run the cells step by step to:

Preprocess data

Train the CNN

Evaluate performance

 Results (Example)

Training Accuracy: ~96%

Validation Accuracy: ~93%

Test Accuracy: ~87%

 Technologies Used

Python

TensorFlow / Keras

NumPy, OpenCV

Matplotlib, Seaborn

scikit-learn
