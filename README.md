# 🧠 Simple-Neural-Network_Basic-Pytorch

This project demonstrates a **basic neural network built using PyTorch** and trained to classify the **MNIST handwritten digits dataset** ✍️.  
It helped me understand the **end-to-end neural network pipeline** and build a strong foundation in **deep learning** 🚀.

---

## 📌 Project Overview

This project is my **first neural network implementation** and serves as a **proof of concept for mastering the PyTorch workflow**.  
It covers the complete lifecycle of a neural network, including:

- 📥 Data loading  
- 🏗️ Model architecture design  
- 🔁 Training loops  
- 📊 Model evaluation  

---

## 📂 Dataset

**MNIST**  
- 🔢 Handwritten digits (**0–9**)  
- 🖼️ **Data Type:** Grayscale images  
- 📐 **Image Size:** \(28 \times 28\) pixels  
- 🧮 **Input Features:** 784 (when flattened)

---

## 🛠️ Tools & Technologies

- 🔥 **PyTorch** – Core framework for building and training the neural network  
- 🧰 **Torchvision** – Dataset downloading and image transformations  
- 🐍 **Python** – Base programming language  

---

## 🚧 Progress Involved

### 1️⃣ Loading the Data
- Imported the MNIST dataset
- Applied image transformations:
  - `ToTensor()` to convert images into tensors
- Split the dataset into:
  - 🏋️ Training set
  - 🧪 Testing set
- Used `DataLoader` for:
  - Efficient batching
  - Data shuffling

---

### 2️⃣ Building the Model
- Created a custom model class inheriting from `nn.Module`
- **Layers:**
  - Used `nn.Linear` layers for feature processing
- **Activation Function:**
  - Integrated **ReLU (Rectified Linear Unit)** ⚡ for non-linearity
- **Forward Function:**
  - Defined how data flows through the network to generate predictions

---

### 3️⃣ Defining Training Logic
- **Loss Function (Criterion):**
  - Used `CrossEntropyLoss` 📉 to measure prediction error
- **Optimizer:**
  - Used optimization algorithms such as:
    - SGD
    - Adam ⚙️  
  - Responsible for updating model weights

---

### 4️⃣ Training the Model
- Trained the model for a fixed number of epochs (`n_epochs`)
- For each batch:
  1. 🔮 Forward pass (prediction)
  2. 📉 Loss computation
  3. 🔁 Backpropagation using `loss.backward()`
  4. 🔧 Weight updates using the optimizer

---

### 5️⃣ Testing & Evaluation
- Loaded the test dataset
- Passed test images through the trained model
- Compared predicted labels with true labels
- Calculated final **accuracy percentage** 📊

---

### 6️⃣ Results 🏆
- ✅ **Accuracy on 10,000 test images:** **97.14%**

---

## 📚 Key Learnings

- 🔄 **Data Pipeline:**  
  Transforming and batching raw image data effectively
- 🏗️ **Model Architecture:**  
  Building structured models using `nn.Module`, linear layers, and activations
- 📊 **Evaluation Process:**  
  Understanding the difference between:
  - Training phase (with gradient computation)
  - Testing phase (evaluation without gradients)

---
