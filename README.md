## Brain Tumor Detection System (MRI-Based)
This project is a **Deep Learning-based Brain Tumor Detection System** that classifies MRI brain images into four categories:

* Glioma Tumor
* Meningioma Tumor
* Pituitary Tumor
* No Tumor

The model is trained using **Convolutional Neural Networks (CNNs)** and deployed with a **Streamlit web application** for easy interaction.

---

## Features

* Upload MRI brain scan images
* Predict tumor type instantly
* Simple and interactive UI using Streamlit
* High accuracy classification model
* Supports 4-class classification

---

## Tech Stack

* **Python**
* **TensorFlow / Keras**
* **NumPy, Pandas**
* **OpenCV / PIL**
* **Streamlit**
* **Google Colab (for training)**

---

## Project Structure

```
Brain-Tumor-Detection/
│
├── model/
│   └── brain_tumor_model.h5
│
├── app.py
├── requirements.txt
├── README.md
└── dataset/ (optional)
```

---

## Step-by-Step Setup Guide

### 1️ Clone the Repository

```bash
git clone https://github.com/your-username/brain-tumor-detection.git
cd brain-tumor-detection
```

---

### 2️ Create Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate     # For Windows
# source venv/bin/activate   # For Mac/Linux
```

---

### 3️ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 4️ Download / Add Trained Model

* You trained the model using **Google Colab**
* Download the `.h5` model file
* Place it inside the `model/` directory

Example:

```
model/brain_tumor_model.h5
```

---

### 5️ Run the Streamlit App

```bash
streamlit run app.py
```

---

### 6️ Open in Browser

After running, Streamlit will provide a local URL like:

```
http://localhost:8501
```

Open it in your browser.

---

## How to Use

1. Upload an MRI image
2. Click on **Predict**
3. The model will classify the image into:

   * Glioma
   * Meningioma
   * Pituitary
   * No Tumor

---

## Model Training (Google Colab)

* Model was trained using MRI dataset in **Google Colab**
* Used CNN architecture for image classification
* Saved model using:

```python
model.save("brain_tumor_model.h5")
```

---

##  Requirements

Example `requirements.txt`:

```
streamlit
tensorflow
numpy
pandas
opencv-python
pillow
```

---

Future Improvements

* Improve model accuracy with larger dataset
* Add Grad-CAM visualization for explainability
* Deploy on cloud (AWS / Heroku / Streamlit Cloud)
* Add patient report generation
