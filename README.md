# Cats vs Dogs Classification using Support Vector Machine (SVM)

## **Objective**
This project implements a **Support Vector Machine (SVM)** to classify images of cats and dogs from the Kaggle **Dogs vs Cats** dataset. The model is trained on a downsampled dataset to improve training efficiency while maintaining a balanced dataset. The goal is to classify new images into one of the two classes: **Cat** or **Dog**.

---

## **Dataset**
- **Source**: [Kaggle - Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats/data)
- **Description**: The dataset contains 25,000 labeled images of cats and dogs. The images are pre-labeled with filenames containing the class (`cat` or `dog`).
- **Size After Downsampling**: The dataset has been downsampled to **2,500 images of cats** and **2,500 images of dogs**, resulting in **5,000 images total** for training the model.

---

## **Workflow**

1. **Data Preprocessing**:
   - Load the images from the dataset.
   - Resize each image to 64x64 pixels.
   - Flatten the images into feature vectors.
   - Normalize pixel values to the range [0, 1].

2. **Downsampling**:
   - The dataset is downsampled to **2,500 cat images** and **2,500 dog images** for balanced training.

3. **Model Training**:
   - Use the **Support Vector Machine (SVM)** classifier with an **RBF kernel**.
   - Split the dataset into an **80-20 training-test split**.
   - Train the model on the training set and evaluate it on the test set.

4. **Model Evaluation**:
   - Evaluate the model using metrics such as **accuracy** and **classification report**.
   - Print out the **classification report** with precision, recall, and F1-score.

---

## **Technologies used**:
  - Language: Python
  - Libraries:
     - numpy
     - cv2 (OpenCV)
     - sklearn (for SVM and model evaluation)
