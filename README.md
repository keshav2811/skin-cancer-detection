# 🩺 Skin Cancer Detection Using Deep Learning

An AI-based skin lesion classification project using Convolutional Neural Networks (CNNs) and the HAM10000 dataset to classify dermatoscopic images into seven different skin lesion categories.

## 📌 Project Overview

Skin cancer is one of the most common forms of cancer worldwide. Early identification and classification of suspicious skin lesions can support timely medical evaluation.

This project explores the application of Deep Learning and Computer Vision to classify skin lesion images using a CNN-based approach.

The model is trained using the **HAM10000 (Human Against Machine with 10,000 training images) dataset**, which contains dermatoscopic images representing seven different categories of skin lesions.

**Important:** This is an academic research project and is not intended to replace professional medical diagnosis.

## 🎯 Objectives

- Develop a deep learning model for skin lesion image classification.
- Apply image preprocessing and data analysis techniques.
- Train a CNN model to recognize different skin lesion categories.
- Evaluate model performance using classification metrics.
- Explore the potential of AI-assisted skin cancer screening.

## 🔬 Dataset

**HAM10000 Dataset**

The project uses the HAM10000 dataset, containing 10,015 dermatoscopic image records.

Dataset classes:

| Label | Skin Lesion Category |
|---|---|
| AKIEC | Actinic Keratoses and Intraepithelial Carcinoma |
| BCC | Basal Cell Carcinoma |
| BKL | Benign Keratosis-like Lesions |
| DF | Dermatofibroma |
| MEL | Melanoma |
| NV | Melanocytic Nevi |
| VASC | Vascular Lesions |

Dataset source: [HAM10000 – Harvard Dataverse](https://doi.org/10.7910/DVN/DBW86T)

## ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| TensorFlow / Keras | Deep learning model development |
| CNN | Image classification |
| NumPy | Numerical computations |
| Pandas | Dataset handling |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Label encoding and evaluation |
| PIL | Image processing |
| Kaggle Notebook | Model development and GPU execution |

## 🧠 Model Architecture

The project implements a Convolutional Neural Network (CNN) using Keras.

The notebook includes the following deep learning components:

- Convolutional layers for feature extraction.
- Max Pooling layers for dimensionality reduction.
- Batch Normalization for training stability.
- Dropout for regularization.
- Flatten layer for feature transformation.
- Dense layers for classification.

**Image input size:** 65 × 65 pixels.

**Output:** Seven skin lesion categories.

## 📂 Repository Structure

```text
skin-cancer-detection/
│
├── FINAL_YEAR_PROJECT.ipynb
│
├── Final_Report_Skin_Cancer_.pdf
│
├── Skin_cancer_Research_Paper.pdf
│
└── README.md
```

## 🚀 Installation and Execution

### 1. Clone the repository

```bash
git clone https://github.com/keshav2811/skin-cancer-detection.git
```

### 2. Navigate to the project directory

```bash
cd skin-cancer-detection
```

### 3. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn pillow scikit-learn tensorflow
```

### 4. Download the dataset

Download the HAM10000 dataset and its metadata file from the official dataset source.

Ensure the following files are available:

- HAM10000_metadata.csv
- HAM10000 image files

### 5. Configure the dataset path

The original notebook uses a Kaggle dataset path:

```python
skin_df = pd.read_csv(
    '/kaggle/input/skin-cancer-lesions-inzip/HAM10000_metadata.csv'
)
```

If running locally, update the path to your downloaded dataset location.

### 6. Run the notebook

Open the notebook:

```bash
jupyter notebook FINAL_YEAR_PROJECT.ipynb
```

Alternatively, upload it to Kaggle or Google Colab, configure the dataset and select a GPU runtime where available.

Execute the notebook cells sequentially.

## 📊 Evaluation Metrics

The model should be evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics help assess classification performance across the seven lesion categories.

Actual performance values should be reported from the executed model rather than assumed.

## 📑 Project Documentation

Additional project documentation is available in this repository:

- **Final Project Report:** `Final_Report_Skin_Cancer_.pdf`
- **Research Paper:** `Skin_cancer_Research_Paper.pdf`
- **Implementation:** `FINAL_YEAR_PROJECT.ipynb`

## 🔮 Future Enhancements

- Experiment with transfer learning architectures such as ResNet50, EfficientNet and MobileNet.
- Introduce image augmentation to improve generalization.
- Address class imbalance using appropriate sampling techniques.
- Develop a Streamlit-based interface for image uploads and predictions.
- Improve model interpretability using Grad-CAM.
- Evaluate performance on independent datasets.

## ⚠️ Disclaimer

This project is developed for educational and research purposes only. Predictions generated by the model must not be considered medical advice or a confirmed diagnosis. Always consult a qualified dermatologist for medical evaluation.

## 👨‍💻 Author

**Keshav Kumar**

M.Tech – Artificial Intelligence & Machine Learning

GitHub: [@keshav2811](https://github.com/keshav2811)

---

⭐ If you find this project interesting, consider giving the repository a star!

