# Fashion-MNIST Classification: CNN vs Random Forest

A Jupyter Notebook project comparing **Convolutional Neural Network (CNN)** and **Random Forest** models on the Fashion-MNIST dataset.

## Overview

This project demonstrates:
- Loading and visualizing the Fashion-MNIST dataset
- Data preprocessing for both CNN and Random Forest
- Training a CNN model using TensorFlow/Keras
- Training a Random Forest model using scikit-learn
- Performance evaluation and comparison
- Confusion matrices and classification reports

## Dataset

**Fashion-MNIST** is a dataset of Zalando's article images consisting of:
- 60,000 training examples
- 10,000 test examples
- 28x28 grayscale images
- 10 classes (T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle Boot)

## Project Structure

```
.
├── demoforcomputervision.ipynb    # Main Jupyter Notebook
├── README.md                      # This file
├── requirements.txt               # Python dependencies
└── (optional) outputs/            # Saved models, plots, etc.
```

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd fashion-mnist-comparison
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate    # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## How to Run

1. Open `demoforcomputervision.ipynb` in Jupyter Notebook
2. Run all cells sequentially
3. The notebook will:
   - Download Fashion-MNIST dataset automatically
   - Train both models
   - Generate visualizations and comparison tables

## Requirements

See `requirements.txt` for full list.

Key libraries:
- TensorFlow / Keras (for CNN)
- scikit-learn (for Random Forest)
- Matplotlib & Seaborn (visualizations)
- Pandas & NumPy (data handling)

## Models Performance (Typical Results)

| Model          | Train Accuracy | Test Accuracy | Training Time |
|----------------|----------------|---------------|---------------|
| CNN            | ~98-99%        | ~91-92%       | ~10-15 min    |
| Random Forest  | ~100%          | ~87-89%       | ~2-5 min      |

**Note:** Exact numbers may vary based on hardware.

## Key Insights

- **CNN** generally outperforms Random Forest on image classification tasks because it preserves spatial hierarchy.
- Random Forest is faster to train but slightly less accurate.
- Common confusions occur between visually similar classes: Shirt, T-shirt/Top, Pullover, Coat.

## Production Recommendation

**Use CNN** for production deployment because:
- Better accuracy
- Scalable with more data
- Can be optimized with TensorFlow Serving / ONNX
- Good for real-time inference on GPU/TPU

Random Forest can be used for quick prototyping or when computational resources are limited.


## Author

Hasil Dayani