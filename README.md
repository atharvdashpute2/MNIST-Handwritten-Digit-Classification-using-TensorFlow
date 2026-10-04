# MNIST-Handwritten-Digit-Classification-using-TensorFlow
A deep learning project using TensorFlow and Keras to classify handwritten digits from 0 to 9 using the MNIST dataset and a neural network.
# MNIST Handwritten Digit Classification using TensorFlow

## 📌 Overview

This project implements a simple **Deep Learning Neural Network** using **TensorFlow and Keras** to recognize handwritten digits from **0 to 9**.

The project uses the popular **MNIST dataset**, which contains 28×28 pixel grayscale images of handwritten digits.

## 🚀 Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* MNIST Dataset

## 📂 Project Structure

```text
MNIST-Digit-Classification-TensorFlow/
│
├── MNIST_Digit_Classification.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

## 🧠 Neural Network Architecture

The model contains the following layers:

```text
Input Image (28 × 28)
        ↓
Flatten
        ↓
Dense Layer (128 neurons)
        ↓
ReLU Activation
        ↓
Dense Layer (10 neurons)
        ↓
Softmax Activation
        ↓
Digit Prediction (0–9)
```

## 📊 Dataset

The project uses the **MNIST handwritten digit dataset** provided by TensorFlow/Keras.

* Training images: 60,000
* Testing images: 10,000
* Image size: 28 × 28 pixels
* Number of classes: 10
* Classes: 0–9

## ⚙️ Data Preprocessing

The pixel values originally range from **0 to 255**.

They are normalized to a range of **0 to 1**:

```python
x_train = x_train / 255.0
x_test = x_test / 255.0
```

The labels are converted into one-hot encoded format using:

```python
to_categorical()
```

## 🔧 Model Configuration

The model uses:

* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy
* **Metric:** Accuracy
* **Epochs:** 5
* **Batch Size:** 32
* **Hidden Layer:** 128 neurons
* **Activation:** ReLU
* **Output Activation:** Softmax

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/MNIST-Digit-Classification-TensorFlow.git
```

### 2. Open the project folder

```bash
cd MNIST-Digit-Classification-TensorFlow
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
MNIST_Digit_Classification.ipynb
```

Run all the cells to train and evaluate the model.

## 📈 Expected Output

After training, the model evaluates its performance on the test dataset and displays the test accuracy.

Example:

```text
Test accuracy: 0.97
```

The exact accuracy may vary slightly depending on the environment and training configuration.

## 🎯 Learning Objectives

This project demonstrates:

* Loading a dataset using TensorFlow
* Image preprocessing
* Data normalization
* One-hot encoding
* Building a Sequential neural network
* Using Dense and Flatten layers
* ReLU and Softmax activation functions
* Model compilation
* Neural network training
* Model evaluation
* Handwritten digit classification

## 🔮 Future Improvements

Possible improvements include:

* Adding Convolutional Neural Networks (CNN)
* Increasing model accuracy
* Adding dropout layers
* Visualizing predictions
* Creating a web interface for handwritten digit recognition
* Allowing users to draw digits and get real-time predictions

## 👨‍💻 Author

**Atharv Dashpute**

## 📄 License

This project is created for educational and learning purposes.
