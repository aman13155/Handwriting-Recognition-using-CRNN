# Handwriting Recognition using CRNN and Keras

A Deep Learning project that recognizes handwritten text from images using a Convolutional Recurrent Neural Network (CRNN) with Connectionist Temporal Classification (CTC) Loss.

## Overview

This project implements a handwriting recognition system using CNN and Bidirectional LSTM layers. It extracts visual features from handwritten images and predicts corresponding text sequences without requiring character-level segmentation.

## Key Features

- Handwritten image recognition
- Image preprocessing and normalization
- Grayscale image processing
- CNN-based feature extraction
- Bidirectional LSTM sequence learning
- CTC Loss for sequence prediction
- Greedy CTC decoding
- Validation and test predictions

## Model Architecture

The project follows this pipeline:

```text
Handwritten Image
       |
       v
Image Preprocessing
(Grayscale, Resize, Normalize)
       |
       v
CNN Feature Extraction
       |
       v
Reshape + Dense Layer
       |
       v
Bidirectional LSTM
       |
       v
Character Prediction
       |
       v
CTC Decoding
       |
       v
Recognized Text
```

## Dataset

**Handwriting Recognition Dataset – Kaggle**

Dataset: https://www.kaggle.com/datasets/landlord/handwriting-recognition

The notebook uses:
- Training images and labels
- Validation images and labels
- Test images

The training pipeline uses 30,000 training samples and 3,000 validation samples.

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Deep Learning

## Model Configuration

| Component | Configuration |
|---|---|
| Input image | 256 × 64 × 1 |
| Feature extraction | CNN |
| Sequence learning | Bidirectional LSTM |
| LSTM units | 256 per direction |
| Output | Character probabilities |
| Loss function | CTC Loss |
| Optimizer | Adam |
| Learning rate | 0.0001 |
| Epochs | 6 |
| Batch size | 128 |

## Installation

Clone the repository:

```bash
git clone https://github.com/aman13155/Handwriting-Recognition-using-CRNN.git
```

Navigate into the project:

```bash
cd Handwriting-Recognition-using-CRNN
```

Install dependencies:

```bash
pip install tensorflow keras opencv-python numpy pandas matplotlib kagglehub
```

## Execution

1. Open the notebook in Kaggle or Jupyter Notebook.
2. Download the dataset from Kaggle.
3. Run the preprocessing cells.
4. Build and train the CRNN model.
5. Evaluate predictions on the validation set.
6. Test handwritten image recognition.

## Evaluation

The notebook evaluates:
- Character-level prediction accuracy
- Word-level prediction accuracy
- Sample predictions on test images

Actual accuracy results can be added after running the notebook.

## Future Improvements

- Increase training dataset size.
- Improve recognition of unclear handwriting.
- Experiment with deeper CNN architectures.
- Improve sequence decoding.
- Deploy the trained model through a web application.

## Author

**Aman Tarikere**

MCA Graduate | AI/ML Enthusiast | Deep Learning

- GitHub: https://github.com/aman13155
- Portfolio: https://a-man.live/
- ORCID: https://orcid.org/0009-0006-9678-9449

---

If you find this project useful, please consider giving it a ⭐ on GitHub!
