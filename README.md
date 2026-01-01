# Image Data Augmentation with Keras

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red?style=flat&logo=keras)

##  Project Overview
In deep learning, having a large and diverse dataset is crucial for model performance. This project implements a **Data Augmentation Pipeline** using `tensorflow.keras.preprocessing.image`. It takes a single input image and automatically generates multiple varied versions of it to artificially expand the size of a training dataset.

##  Transformations Applied
The `ImageDataGenerator` is configured to apply the following random transformations:
* **Rotation:** Randomly rotates images up to 40 degrees.
* **Width/Height Shifts:** Shifts the image horizontally or vertically by 20%.
* **Shear & Zoom:** Applies shearing transformations and random zooms.
* **Horizontal Flip:** Randomly flips images horizontally.
* **Fill Mode:** Uses 'nearest' pixel filling to handle newly created pixels.

##  Tech Stack
* **Deep Learning:** TensorFlow, Keras
* **Image Processing:** NumPy, Matplotlib
* **File Handling:** OS module

##  How It Works
1.  **Load Image:** The script loads a sample image from the local directory.
2.  **Preprocess:** Converts the image to a NumPy array and reshapes it for the model.
3.  **Generate:** The generator creates 40 unique augmented versions of the original image.
4.  **Save:** All generated images are saved automatically to a specified output folder (e.g., `augmented_images`).

## How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/PyPro2024/Image-Data-Augmentation-Keras.git]
    ```
2.  **Install dependencies:**
    ```bash
    pip install tensorflow numpy matplotlib
    ```
3.  **Run the Notebook:**
    Open `Data_Augmentation.ipynb`, update the `img_path` to point to your image, and run the cells.

---
*This project demonstrates essential preprocessing techniques for Computer Vision tasks.*
