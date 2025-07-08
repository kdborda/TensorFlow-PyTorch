# EM Lab03: TensorFlow vs PyTorch

This repository contains the implementation and comparison of a simple neural network trained on the MNIST dataset using both **TensorFlow** and **PyTorch**. It was developed as part of the **Embedded Machine Learning Lab (EM Lab03)** at TH Deggendorf – Campus Cham, under the guidance of **Prof. Tobias Schaffer**.

---

## 🧠 Objective

* Build and train the same neural network in both TensorFlow and PyTorch
* Compare training time and performance
* Convert the models for embedded deployment:

  * **TensorFlow Lite** (`.tflite`)
  * **ONNX** (`.onnx`)

---

## 💠 Lab Tasks

### 1. Model Implementation and Training

* Load and preprocess MNIST dataset (28×28 grayscale images)
* Define a simple architecture:

  * Input layer (784 features)
  * Dense layer with 64 ReLU units
  * Output layer with 10 classes
* Train for 5 epochs
* Measure training time

### 2. Inference and Evaluation

* Run inference on test set
* Measure test accuracy and inference time

### 3. Model Conversion

* Export trained TensorFlow model to **TensorFlow Lite**
* Export trained PyTorch model to **ONNX**

---

## 📂 Contents

* `Lab03 TensorFlow vs PyTorch.ipynb` – Jupyter notebook with full implementation
* `model.tflite` – Converted TensorFlow Lite model
* `model.onnx` – Exported PyTorch model in ONNX format
* `training_logs/` – (Optional) Folder containing logs
* `report.md` – Short comparison of frameworks

---

## 📊 Comparison Highlights

| Feature           | TensorFlow             | PyTorch                  |
| ----------------- | ---------------------- | ------------------------ |
| Code Structure    | Sequential & concise   | Modular & explicit       |
| Training Speed    | Fast                   | Slightly slower          |
| Inference Speed   | Comparable             | Comparable               |
| Export Simplicity | Easy (TFLiteConverter) | Easy (torch.onnx.export) |

---

## ✅ Requirements

* Python 3.8+
* TensorFlow ≥ 2.x
* PyTorch ≥ 1.10
* torchvision
* numpy

Install dependencies:

```bash
pip install tensorflow torch torchvision numpy
```

---

## 📌 License

This project is provided for academic and educational use. Attribution to **TH Deggendorf – Prof. Tobias Schaffer** is appreciated.
