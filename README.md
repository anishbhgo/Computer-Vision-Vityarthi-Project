# MNIST Digit Recognition & Optical Character Recognition (OCR)

## Project Overview
This project, developed by **Anish Bhattacharjee**, focuses on **Optical Character Recognition (OCR)** and **Handwritten Digit Classification**. It combines traditional computer vision techniques with deep learning to extract and identify text from images. Specifically, the project utilizes a **Multi-Layer Perceptron (MLP)** trained on the **MNIST dataset** to recognize handwritten digits with high accuracy.

---

## Author Information
* **Lead Developer**: Anish Bhattacharjee
* **Affiliation**: B.Tech 3rd-year student at VIT Bhopal University
* **Registration Number**: 23BAI10736
* **Contact**: anish.23bai10736@vitbhopal.ac.in | 8011791812

---

## Technical Analysis

### 1. Digit Recognition (MNIST)
The core of the project is a neural network built using the **Keras API**.
* **Model Architecture**: A four-layer `Sequential` network with 8,600 trainable parameters.
* **Layers**: Includes three hidden layers (10, 30, and 10 nodes) using **ReLU** activation and a 10-node output layer with **Softmax**.
* **Performance**: Achieved a test accuracy of approximately **93.18%**.
* **Preprocessing**: Features normalization (scaling pixels to [0,1]), flattening $28 \times 28$ images into 784-pixel vectors, and one-hot encoding for categorical labels.

### 2. OCR Pipeline & Tools
The project evaluates various OCR engines for broader text extraction tasks:
* **PyTesseract**: A Python wrapper for the Tesseract-OCR engine, noted for being simple and powerful.
* **EasyOCR**: Lightweight and efficient for multi-language documents and PDFs.
* **Keras-OCR**: A user-friendly deep learning approach built on TensorFlow.
* **Cloud Solutions**: Includes Amazon Textract, Google Cloud Vision, and Microsoft Azure for high-accuracy, scalable processing.

---

## Applications
* **Image-to-Text**: Direct extraction of printed text from image files.
* **Document Digitization**: Converting scanned documents into machine-readable digital text.
* **Handwriting Recognition**: Transforming handwritten notes into digital formats.
* **Project Integration**: These techniques build upon previous work such as CNN-based object detection and water quality monitoring projects.

---

## Requirements
To run the project environments, ensure the following are installed:
* **System Tools**: `tesseract-ocr`, `libtesseract-dev`.
* **Python Libraries**:
    * `tensorflow` / `keras` (Deep Learning)
    * `pytesseract` (OCR)
    * `opencv-python` (`cv2`) (Image Processing)
    * `pillow` & `matplotlib` (Visualization/Handling)

---

## Usage
Open the provided Jupyter notebooks or `.ipynb` files in **Google Colab**, **Kaggle**, or a local environment to train the model or test text extraction on custom images.

## References
* [HuggingFace Image-to-Text Tasks](https://huggingface.co/tasks/image-to-text)
* [Keras OCR Examples](https://keras.io/examples/vision/captcha_ocr/)
* [Tesseract-OCR GitHub](https://github.com/tesseract-ocr/tesseract)
