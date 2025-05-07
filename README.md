# HandWrittenDigitRecognizer
# Handwritten Digit Recognizer in Java

This project is a Java-based implementation of a **handwritten digit recognition system** using a custom-built neural network. It is trained on the **MNIST dataset** and is capable of recognizing digits from input images using **OpenCV** for image preprocessing.

---

## 📌 Features

- Built-from-scratch neural network in Java
- MNIST training and evaluation
- Image input and digit prediction using OpenCV
- Model saving and loading
- Custom activation functions and backpropagation
- Lightweight and educational

---

## 🧠 Technologies Used

- Java 8+
- OpenCV (for image preprocessing)
- IDX Parser (for reading MNIST dataset files)
- Basic Java I/O and serialization

---

## 🗂️ Project Structure
handwritten-digit-recognizer/
├── src/
│ ├── Main.java
│ ├── NeuralNetwork.java
│ ├── DigitRecognizer.java
│ ├── ImageProcessor.java
│ ├── ModelSaver.java
│ └── utils/
│ └── IDXReader.java
├── model/
│ └── saved_model.json
├── images/
│ └── test_digit.png
├── README.md
└── pom.xml (if using Maven)

