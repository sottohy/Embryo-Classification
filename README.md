# Embryo Classification Model Using Transfer Learning

This project aims to develop a model that aids in the IVF process by classifying embryo images as good or bad, depending on the presence of blastocysts. The model uses transfer learning with ResNet101 to achieve high accuracy.


## Link to the dataset: https://osf.io/3kc2d/


## Project Overview
The goal of this project is to improve the efficiency, precision, and success rates of IVF procedures by automating the classification of embryo images. The model classifies images as either blastocysts (good) or non-blastocysts (bad).



## Data Description
The dataset used in this project consists of embryo images classified into four folders: ED1, ED2, ED3, and ED4. The classification criteria are as follows:

- ED1, ED2, ED4: These folders use a 5-category system.
  - Folders 1, 2: Non-blastocysts
  - Folders 3, 4, 5: Blastocysts
- ED3: This folder uses a 2-category system.
  - Folder 1: Blastocysts
  - Folder 2: Non-blastocysts



## Dependencies
The project requires the following libraries:

- pandas
- scikit-learn
- pillow
- matplotlib
- torch
- torchvision



## Data Preprocessing
1. Loading Data: The embryo images are loaded from the specified directories.
2. Data Augmentation: Augmentation techniques are applied to increase the dataset size, including horizontal flipping, rotation, brightness adjustment, and contrast adjustment.

### Data Augmentation Script
The script for data augmentation performs the following steps:

- Flips the image horizontally.
- Rotates the image by 90 degrees.
- Adjusts brightness and contrast randomly.
- Saves the augmented image to the appropriate output folder.



## Modeling
###Model Selection
The ResNet101 model was chosen due to its proven performance in similar classification tasks. The model was fine-tuned using the preprocessed and augmented dataset.

### Training, Testing, and Evaluation
- Training: The model was trained using the processed dataset, achieving a high accuracy.
- Testing: The model's performance was evaluated on a test set, resulting in a test accuracy of 93%.

### Results
- Confusion Matrix: The confusion matrix for the test results is provided below.
![malak cm 93](https://github.com/sottohy/Embryo-Classification/assets/91037437/c22c6efa-bd88-48b8-ac92-df85c42fde4c)

- Accuracy Plot: The accuracy plot shows the model's performance during training and testing.
![malak accuracy 93](https://github.com/sottohy/Embryo-Classification/assets/91037437/e9c347fa-2507-48f2-bdff-60ade59ae6d3)



## Usage
To run this project, follow these steps:

- Install the required dependencies.
- Load the dataset from the specified paths.
- Execute the provided notebook to preprocess the data, perform data augmentation, train the model, and evaluate its performance.


## Creating the Website
The website for this project is currently under development. It will be created using HTML, CSS, and Flask to connect the model for real-time embryo classification.



##Demo of the Website
![Screenshot (2584)](https://github.com/sottohy/Embryo-Classification/assets/91037437/8e65a352-c04f-426c-ab87-67f2e4067442)

![Screenshot (2585)](https://github.com/sottohy/Embryo-Classification/assets/91037437/268a591f-561b-4a1e-8e14-3996342992b2)

