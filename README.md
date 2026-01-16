# Simple-Neural-Network_Basic-Pytorch
This project demonstrates a basic NN made with pytorch and used to classfiy the MNIST dataset. This project helped me get an idea of the general NN pipeline and develop a footing into the world of deep learning.

# Project Overview

This project is my **first neural network implementation** and serves as a **proof of concept for mastering the PyTorch workflow**. It covers the complete pipeline of a neural network, including data loading, model architecture design, training loops, and evaluation.

---

## Dataset

**MNIST**  
- A large database of handwritten digits (**0–9**)
- **Data Type:** Grayscale images  
- **Image Size:** \(28 \times 28\) pixels  
- **Input Features:** 784 (when flattened)

---

## Tools & Technologies

- **PyTorch** – Core framework for building and training the neural network  
- **Torchvision** – Used for dataset downloading and image transformations  
- **Python** – Base programming language  

---

## Progress Involved

### 1. Loading the Data
- Imported the MNIST dataset
- Applied image transformations using:
  - `ToTensor()` to convert images into tensors
- Split the dataset into:
  - Training set
  - Testing set
- Used `DataLoader` for:
  - Efficient batching
  - Shuffling the data

---

### 2. Building the Model
- Created a custom model class inheriting from `nn.Module`
- **Layers:**
  - Used `nn.Linear` layers for feature processing
- **Activation Function:**
  - Integrated **ReLU (Rectified Linear Unit)** between layers for non-linearity
- **Forward Function:**
  - Defined how input data flows through layers to produce predictions

---

### 3. Defining Training Logic
- **Loss Function (Criterion):**
  - Used `CrossEntropyLoss` to measure prediction error
- **Optimizer:**
  - Selected optimization algorithms such as:
    - SGD
    - Adam  
  - Responsible for updating model weights

---

### 4. Training the Model
- Trained the model for a defined number of epochs (`n_epochs`)
- For each batch:
  1. Forward pass to predict outputs
  2. Compute loss
  3. Backpropagation using `loss.backward()`
  4. Update weights using the optimizer

---

### 5. Testing & Evaluation
- Loaded the test dataset
- Passed test data through the trained model
- Compared predicted labels with actual labels
- Calculated final **accuracy percentage**

---

### 6. Results
- Accuracy of the newtork on the 10000 test images: 97.14%

---

## Key Learnings

- **Data Pipeline:**  
  Understanding how to transform and batch raw image data for neural networks
- **Model Architecture:**  
  Designing structured models using `nn.Module`, linear layers, and activation functions
- **Evaluation Process:**  
  Differentiating between:
  - Training phase (with gradient computation)
  - Testing phase (accuracy evaluation without gradients)

---
