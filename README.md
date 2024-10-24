# Chest X-Ray Images (Pneumonia) Classification

This project is focused on classifying chest X-ray images to detect pneumonia using a deep learning model based on the DenseNet architecture. The main work is documented in the Jupyter notebook provided in this repository, which walks through the process of loading the dataset, building the model, training it, and evaluating its performance.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model](#model)
- [How to Use](#how-to-use)
- [Validation Set Revision](#validation-set-revision)
- [Results](#results)
- [License](#license)

## Project Overview

This project uses the DenseNet architecture to classify X-ray images into two categories: **NORMAL** and **PNEUMONIA**. The notebook covers the entire workflow, from loading the dataset to training and evaluating the model.

## Dataset

The dataset used in this project is the [Chest X-Ray Images (Pneumonia) dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) from Kaggle. It consists of X-ray images categorized as **NORMAL** or **PNEUMONIA**. The dataset is divided into training, validation, and test sets, which are used throughout the notebook to train and evaluate the model.

## Model

The model is built using the **DenseNet121** architecture, pre-trained on ImageNet. The final layer is modified to classify the images into two classes (NORMAL and PNEUMONIA). Additional layers are also added, including dropout and fully connected layers, to enhance model performance.

## How to Use

To explore the project:

1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/your-repo-name.git
2. Open the notebook in Jupyter or Google Colab:
   - The entire workflow is contained in the notebook, including data loading, model building, training, and evaluation.

## Validation Set Revision

Originally, the dataset had only 16 images in the validation set, which was insufficient for effective model evaluation. To improve the validation process, I redistributed images from the training set to the validation set, ensuring a more balanced and representative validation set. This modification allows for more reliable validation metrics and a better understanding of the model's performance during training.

## Results

After training the DenseNet model, I achieved a validation accuracy of **96%**. Additional metrics like **F1-score**, **Precision**, and **Recall** were also calculated to further evaluate the model's performance. Confusion matrices were generated to provide more insight into the model's predictions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
