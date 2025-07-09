# ChestX-Pneumonia-CNN: Pneumonia Detection from Chest X-ray Images using Convolutional Neural Networks

## Overview

Pneumonia is a severe lung infection that inflames the air sacs in one or both lungs, often filling them with fluid or pus. It is a leading cause of death worldwide, especially among young children. Traditional diagnosis through chest X-rays can be challenging even for skilled radiologists, and manual analysis can be time-consuming and prone to human error.

This project leverages the power of Convolutional Neural Networks (CNNs) to automate and enhance the detection of pneumonia from chest X-ray images. By training a deep learning model on a vast dataset of chest X-rays, this system aims to provide a highly accurate and efficient tool for assisting in the early diagnosis of pneumonia.

## Motivation

The high prevalence and severity of pneumonia underscore the critical need for accurate and timely detection. By integrating machine learning algorithms, particularly CNNs, into the diagnostic process, we can:
* Increase the efficacy and reach of the diagnosis procedure.
* Potentially reduce human error in interpreting X-ray images.
* Automate a time-consuming diagnostic step, allowing medical professionals to focus on treatment.

## Features

* **Pneumonia Detection:** Classifies chest X-ray images as either "Normal" or "Pneumonia."
* **Convolutional Neural Network (CNN) Model:** Utilizes a robust CNN architecture (e.g., VGG19 with custom layers as indicated by search results, though the specific architecture of *your* repository would be more accurate if available in your `README.md` file) for image classification.
* **User-Friendly Web Application:** A Streamlit-based web interface for easy interaction, allowing users to upload X-ray images and receive real-time predictions.
* **Data Augmentation:** Employs techniques like horizontal flip, height/width shift, rotation, shear, and zoom to enhance model generalization.

## Technologies Used

* **Python**
* **TensorFlow** (2.4.1+)
* **Keras** (2.4.3+)
* **scikit-learn** (0.24.1+)
* **matplotlib** (3.3.3+)
* **texttable** (1.6.3+)
* **Gradio** (1.5.3+)
* **Streamlit** (for the web application)

## Dataset

The model is trained on a dataset of chest X-ray images categorized into "Normal" and "Pneumonia" classes. The dataset is typically split into training, testing, and validation sets.

* **Training Set:** ~1341 Normal, ~3875 Pneumonia images
* **Test Set:** ~234 Normal, ~390 Pneumonia images
* **Validation Set:** ~8 Normal, ~8 Pneumonia images

*(Note: These numbers are based on common datasets used for this problem, specific counts might vary based on your exact dataset split.)*

## Installation and Setup

To set up and run the project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/anoshandrews/ChestX-Pneumonia-CNN.git](https://github.com/anoshandrews/ChestX-Pneumonia-CNN.git)
    cd ChestX-Pneumonia-CNN
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Ensure you have a `requirements.txt` file in your repository listing all necessary libraries and their versions.)*

4.  **Prepare the dataset:**
    Copy the `chest-xray` directory contents (containing `train`, `test`, and `val` subdirectories) into a `data` folder within the project root.

5.  **Train the model (optional):**
    If you wish to train the model from scratch, execute the relevant Python script (e.g., `model_training.py` or a Jupyter notebook) from the `source` directory.

## Usage (Web Application)

To run the Streamlit web application locally:

1.  Navigate to the `webapp` directory:
    ```bash
    cd webapp
    ```

2.  Run the Streamlit application:
    ```bash
    streamlit run web_app.py
    ```

3.  Open your web browser and go to the URL provided by Streamlit (usually `http://localhost:8501`). You can then upload a new X-ray image or select from provided examples to get a pneumonia prediction.

## Live Demo

Experience the ChestX-Pneumonia-CNN live application here:

[ChestX-Pneumonia Live Demo](https://chestx-pneumonia.streamlit.app/)

## License

This project is licensed under the Apache-2.0 License. See the `LICENSE` file for more details.

---
