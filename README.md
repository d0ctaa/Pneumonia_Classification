# PyTorch - ResNet50 Image Classification.
PyTorch

##### This project demonstrates the process of training, evaluating, and testing a deep learning model for classifying chest X-ray images into two categories: Normal and Pneumonia. 
##### The project uses a ResNet50 model with custom modifications and leverages Google Colab for GPU acceleration.

> The data was acquired trough kaggle.
> Original Data Can be accessed on Kaggle Here:  https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images?utm_medium=social&utm_campaign=kaggle-dataset-share&utm_source=twitter

Chest X-Ray Classification using ResNet50


Table of Contents

1. Installation
2. Data Preparation
3. Model Architecture
4. Training
5. Evaluation
6. Testing
7. Results
8. References

=======================================================================================================

1. Installation

To run this project,Ensure you have torchmetrics installed:
- pip install torchmetrics
  
2. Data Preparation

* Mount Google Drive:
> Mount your Google Drive to access the dataset.

* Define Transforms:

> Define the transformations to be applied to the images, including resizing, grayscaling, random rotations, flips, and normalization.

* Load Dataset:

> Load the training and testing datasets using torchvision.datasets.ImageFolder.

* Create Validation Set:

> Split the main dataset into training and validation sets.

* Create Data Loaders:

> Create data loaders for the training, validation, and test sets.

3. Model Architecture

* Instantiate and Modify Model:

> Instantiate the ResNet50 model and add dropout layers for regularization.

4. Training

- Define Loss Function and Optimizer:

> Use CrossEntropyLoss as the loss function and SGD as the optimizer.

- Training Loop:

> Train the model over several epochs, tracking loss values.

5. Evaluation

* Save and Load Model:

> Save the trained model to Google Drive and load it for evaluation.

- Evaluation Loop:

> Evaluate the model on the validation set, computing metrics such as accuracy and ROC-AUC.

6. Testing

* Testing Loop:

> Test the model on the test set and compute evaluation metrics.

7. Results

* Training Loss:

> The training loss decreases significantly over 50 epochs, indicating successful training.

* Validation Metrics:

  - Accuracy: 97.91%
  - ROC-AUC: 99.70%
* Test Metrics:

  - Accuracy: 91.19%
  - ROC-AUC: 99.21%

8. References

- PyTorch Documentation
- TorchMetrics Documentation
- ResNet50 Paper
- Chest X-ray Dataset: https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images?utm_medium=social&utm_campaign=kaggle-dataset-share&utm_source=twitter
- For more details, refer to the code in this repository.
