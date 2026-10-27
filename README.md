# Cat vs Dog Image Classification using CNN

A TensorFlow/Keras Convolutional Neural Network (CNN) project that classifies images as **Cat** or **Dog**.

## Features
- Automatically locates the `PetImages/Cat` and `PetImages/Dog` dataset folders in common Kaggle and Colab locations.
- Resizes images to 150 × 150 and normalizes pixel values.
- Uses an 80/20 training/validation split.
- Applies random horizontal flips and small rotations during training.
- Uses early stopping and saves the best model checkpoint.
- Plots training/validation accuracy and loss.
- Displays sample predictions with confidence scores.

## Dataset
This project uses the Microsoft Cats vs Dogs image dataset distributed through Kaggle. The dataset is not included in this repository because it is large. Download it from Kaggle and attach it as an input in Kaggle Notebooks, or extract it in Colab so the folder structure is:

```text
PetImages/
├── Cat/
└── Dog/
```

The notebook searches common Kaggle and Colab locations automatically. If your dataset is stored elsewhere, update `DATA_DIR` detection in the notebook.

## Run the notebook
1. Open `CatDogImageClassification.ipynb` in Google Colab or Kaggle.
2. Attach/download the dataset and ensure the `PetImages/Cat` and `PetImages/Dog` folders are available.
3. Run the cells from top to bottom. A GPU is recommended but not required.
4. The notebook saves `best_cat_dog_model.keras` and `cat_dog_cnn.keras` in the current runtime.

## Requirements
See [`requirements.txt`](requirements.txt). TensorFlow is the main dependency.

## Important evaluation note
The notebook reports **validation** metrics from an 80/20 split. Do not describe these as independent test accuracy. Add the actual metrics after running the notebook; no performance score is claimed in advance.
