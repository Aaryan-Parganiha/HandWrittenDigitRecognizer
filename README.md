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

2. Setup OpenCV
Ensure OpenCV is installed and properly linked in your IDE or build tool (like Maven or Gradle).

You can download OpenCV from opencv.org.

3. Run the Project
Compile and run the Main.java file from your IDE or via terminal:

bash
Copy
Edit
javac -cp .:path/to/opencv.jar src/Main.java
java -cp .:path/to/opencv.jar Main
Replace path/to/opencv.jar with the actual path to your OpenCV .jar file.

🧪 Usage
🏋️ Train the Model
Train the neural network using the MNIST .idx dataset files:

java
Copy
Edit
NeuralNetwork nn = new NeuralNetwork(784, 64, 10);
nn.train(trainImages, trainLabels, epochs);
ModelSaver.saveModel(nn, "model/saved_model.json");
📸 Recognize a Digit
Use OpenCV to preprocess and predict digits from external images:

java
Copy
Edit
DigitRecognizer recognizer = new DigitRecognizer("model/saved_model.json");
int prediction = recognizer.predict("images/test_digit.png");
System.out.println("Predicted Digit: " + prediction);

📂 Dataset
Download MNIST dataset files from Yann LeCun's website:

train-images-idx3-ubyte

train-labels-idx1-ubyte

t10k-images-idx3-ubyte

t10k-labels-idx1-ubyte

📊 Accuracy
With appropriate training (5+ epochs and ~64 hidden nodes), this model achieves around 90–95% accuracy on MNIST test data.

✍️ Authors
Aaryan Parganiha
Ishaan
Ayush Goel
Deepak
Under the guidance of The NorthCap University
