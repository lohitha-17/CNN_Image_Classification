# CNN-Based Image Classification

## Overview
This project uses Convolutional Neural Networks (CNNs) to classify images from two datasets:
- **MNIST Fashion**: Grayscale images of clothing items into 10 categories.
- **CIFAR-10**: Color images of objects into 10 categories.

The CNNs are designed to be comparable in size to previously implemented Artificial Neural Networks (ANNs) for the same datasets. The project includes model comparison and performance evaluation.

## Objectives
- Build and train CNN models optimized for classification.
- Compare CNN performance with similarly-sized ANN counterparts.
- Evaluate performance using metrics like accuracy, confusion matrices, and F1-scores.

## Datasets
- [MNIST Fashion](https://github.com/zalandoresearch/fashion-mnist)
- [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)

## Features
- Data preprocessing and normalization.
- Experimentation with CNN architectures (convolutional, pooling layers).
- Hyperparameter tuning for performance optimization.
- Comparison of ANN vs CNN on various metrics.

## Results
- **MNIST Fashion**:
  - CNN Accuracy: **89%**
  - Comparison Table:
    | Model Type | Parameters | Train Time (s) | Test Accuracy | Test F1-Score |
    |------------|------------|----------------|---------------|----------------|
    | ANN        | 128,000    | 30             | 88%           | 0.87           |
    | CNN        | 125,000    | 25             | 89%           | 0.88           |

- **CIFAR-10**:
  - CNN Accuracy: **48%**
  - Comparison Table:
    | Model Type | Parameters | Train Time (s) | Test Accuracy | Test F1-Score |
    |------------|------------|----------------|---------------|----------------|
    | ANN        | 256,000    | 45             | 47%           | 0.45           |
    | CNN        | 250,000    | 40             | 48%           | 0.46           |

## Technologies Used
- Python
- TensorFlow/Keras
- NumPy
- Matplotlib

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/CNN_Image_Classification.git
   ```
2. Open `MNIST_Fashion_CNN.ipynb` or `CIFAR10_CNN.ipynb` in Jupyter Notebook or Colab.
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook to reproduce results.

## Challenges and Insights
- **Challenges**: Fine-tuning CNN architectures for optimal performance while maintaining comparable size with ANNs.
- **Insights**: CNNs outperform ANNs for image data due to better feature extraction capabilities.
