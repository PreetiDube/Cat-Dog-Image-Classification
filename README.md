# Cat vs Dog Image Classification using CNN

A deep learning project built with **TensorFlow and Keras** that uses a Convolutional Neural Network (CNN) to classify images as **Cat** or **Dog**.

## Features

- Automatically detects the `PetImages/Cat` and `PetImages/Dog` dataset folders in common Kaggle and Google Colab locations.
- Resizes images to `150 × 150` pixels and normalizes pixel values.
- Uses an 80/20 training-validation split.
- Applies data augmentation through random horizontal flips and small rotations during training.
- Uses early stopping and saves the best model checkpoint.
- Visualizes training and validation accuracy and loss.
- Displays sample predictions with confidence scores.

## Tech Stack

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pillow

## Dataset

This project uses the **Microsoft Cats vs Dogs image dataset**, distributed through Kaggle.

The dataset is not included in this repository because of its size.

**Download the dataset:**
- [Kaggle — Cats vs Dogs](https://www.kaggle.com/competitions/dogs-vs-cats/data)
- [Microsoft Cats vs Dogs dataset](https://www.microsoft.com/en-us/download/details.aspx?id=54765)

After downloading and extracting the dataset, ensure the directory structure is similar to the following:

```text
PetImages/
├── Cat/
│   ├── 1.jpg
│   └── ...
└── Dog/
    ├── 1.jpg
    └── ...
```

The notebook searches common Kaggle and Colab locations automatically. If your dataset is stored elsewhere, update the `DATA_DIR` configuration in the notebook.

## How to Run

1. Open `CatDogImageClassification.ipynb` in Google Colab or Kaggle Notebooks.
2. Attach the dataset in Kaggle or extract it in the Colab runtime.
3. Confirm that the `PetImages/Cat` and `PetImages/Dog` folders are accessible.
4. Run the notebook cells from top to bottom.
5. Review the training curves and sample predictions.

A GPU is recommended to speed up training, but it is not required.

## Model Outputs

After running the notebook, the following model files are saved in the current runtime:

- `best_cat_dog_model.keras` — best model checkpoint.
- `cat_dog_cnn.keras` — final saved model.

These files are generated during training and are not included in the repository by default.

## Evaluation

The notebook uses an **80/20 training-validation split** to evaluate model performance.

Validation metrics should not be described as independent test accuracy. Actual accuracy and loss values should be added here only after the notebook has been executed successfully.

## Installation Requirements

See [`requirements.txt`](requirements.txt) for the project dependencies.

TensorFlow is the primary deep learning dependency.

## Future Improvements

- Improve classification performance through model tuning.
- Experiment with transfer learning using pretrained CNN architectures.
- Add a user-friendly interface for uploading and classifying images.
- Evaluate the trained model on a separate, independent test dataset.

## Author

**Preeti Dube**

- GitHub: [PreetiDube](https://github.com/PreetiDube)
- Project Repository: [Cat-Dog-Image-Classification](https://github.com/PreetiDube/Cat-Dog-Image-Classification)
