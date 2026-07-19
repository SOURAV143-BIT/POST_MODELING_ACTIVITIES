# 👕 Fashion MNIST Image Classification using TensorFlow & Keras

A Deep Learning project that classifies grayscale images of fashion products into one of 10 clothing categories using a Fully Connected Neural Network (FCNN) built with TensorFlow and Keras.

---

## 📌 Project Overview

The Fashion MNIST dataset is a benchmark dataset introduced by Zalando, consisting of 70,000 grayscale images of fashion products. Each image is 28×28 pixels and belongs to one of 10 clothing categories.

The objective of this project is to build, train, evaluate, save, and reload a Deep Neural Network capable of accurately classifying these fashion items.

---

## 🎯 Objectives

- Load the Fashion MNIST dataset
- Visualize sample images
- Normalize image pixel values
- Convert labels into categorical format
- Build a Fully Connected Neural Network (FCNN)
- Train the model using TensorFlow/Keras
- Monitor training with TensorBoard
- Evaluate model performance
- Save the trained model
- Load the saved model and verify its architecture
- Make predictions on unseen test images

---

## 📂 Dataset

**Dataset:** Fashion MNIST

- Training Images: **60,000**
- Testing Images: **10,000**
- Image Size: **28 × 28 pixels**
- Image Type: **Grayscale**
- Number of Classes: **10**

### Classes

| Label | Category |
|--------|----------|
| 0 | T-shirt/Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

## 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- TensorBoard
- Google Colab

---

## 📁 Project Structure

```
Fashion-MNIST-Classification/
│
├── Fashion_MNIST.ipynb
├── fashion_mnist_model.keras
├── README.md
├── logs/
│   └── fit/
└── images/
```

---

## 🔄 Workflow

1. Import Libraries
2. Load Fashion MNIST Dataset
3. Visualize Sample Images
4. Normalize Pixel Values
5. One-Hot Encode Labels
6. Build Neural Network
7. Compile Model
8. Train Model
9. Monitor Training using TensorBoard
10. Evaluate Performance
11. Plot Accuracy & Loss Graphs
12. Save Trained Model
13. Load Saved Model
14. Verify Model Parameters
15. Predict Test Images

---

## 🧠 Model Architecture

```
Input Layer (28 × 28)

        │

Flatten Layer

        │

Dense (512) → ReLU

        │

Dense (256) → ReLU

        │

Dense (128) → ReLU

        │

Dense (10) → Softmax
```

---

## ⚙️ Model Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Activation (Hidden Layers) | ReLU |
| Output Activation | Softmax |
| Epochs | 20 |
| Batch Size | 128 |
| Validation Split | 20% |

---

## 📊 Results

The model achieved approximately:

- **Training Accuracy:** ~90–93%
- **Validation Accuracy:** ~88–91%
- **Test Accuracy:** ~88–91%

Performance may vary slightly depending on random initialization and training conditions.

---

## 📈 Visualizations

The project includes:

- Sample Fashion Images
- Training Accuracy vs Validation Accuracy
- Training Loss vs Validation Loss
- Predicted vs Actual Images
- TensorBoard Training Logs

---

## 💾 Model Saving

The trained model is saved in the Keras format:

```
fashion_mnist_model.keras
```

This file stores:

- Model Architecture
- Learned Weights
- Optimizer State

---

## 🔄 Model Loading

The saved model can be loaded using:

```python
from tensorflow.keras.models import load_model

model = load_model("fashion_mnist_model.keras")
```

After loading, the project verifies:

- Model Architecture
- Number of Parameters
- Weight Shapes
- Prediction Consistency

---

## ▶️ How to Run

1. Clone this repository:

```bash
git clone https://github.com/your-username/Fashion-MNIST-Classification.git
```

2. Open the notebook in Google Colab or Jupyter Notebook.

3. Install the required libraries (if needed):

```bash
pip install tensorflow matplotlib numpy
```

4. Run all notebook cells.

5. Launch TensorBoard to visualize the training process.

---

## 📚 Learning Outcomes

Through this project, you will learn:

- Image preprocessing
- Data normalization
- One-Hot Encoding
- Artificial Neural Networks (ANN)
- TensorFlow & Keras
- Multi-Class Classification
- Model Evaluation
- TensorBoard Visualization
- Saving and Loading Models

---

## 🚀 Future Improvements

- Implement Convolutional Neural Networks (CNN)
- Apply Data Augmentation
- Use Dropout Layers to reduce overfitting
- Hyperparameter Tuning
- Improve Classification Accuracy
- Deploy the model as a web application using Streamlit or Flask

---

## 👨‍💻 Author

**SOURABH**

Bachelor of Computer Applications (BCA)

Aspiring Data Scientist

GitHub: https://github.com/SOURAV143-BIT

---

## ⭐ If you found this project helpful, consider giving it a Star!
```
