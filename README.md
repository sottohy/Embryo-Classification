# Embryo classification model using Transfer Learning

## Classification model for embryo images depending on the presence of blastocysts
## Link to the dataset: https://osf.io/3kc2d/

#### The motivation behind this project is to develop a model that aids in the IVF process by classifying embryo images as good or bad. The goodness or badnees of the images depend on whether the embryo is a blastocyst or not, respectively. The main idea of the project is to create a model designed for the selection phase in the IVF process. This model aims to improve the efficiency, precision, and success rates of IVF procedures by eliminating the human error factor.

## Preprocessing
The original data was classified into four folders, where each folder contained two main things: a folder that has the images (allimagees), and a file that contains the paths to these images with their corresponding labels (target). 

For the folders named ed1 and ed2, the labels were classified into 0/1/2/3. 0/1 refer to non-blastocysts, while 2/3/4 refer to blastocysts.

For the folders named ed3 and ed4, the labels were classified into 0/1. 0 refers to non-blastocysts, while 1 refers to blastocysts.

In preprocessing_embryo_dataset.ipynb: The dataset was read and classified into "good" and "bad" folders using ImageDataGenerator. The good folder contained 834 images and the bad folder contained 627 images. Data augmentation was performed on both classes where rotation and flipping were applied, resulting in a total of 1551 images for the good folder and 1113 images for the bad folder.

## Data Splitting
The images were split into training and testing with a split ratio of 80% train and 20% test, then the train was further split into training and validation with a split ratio of 20%.

## Model Selection & Architecture
The chosen model was ResNet101, as it was previously used in similar cases and resulted in the highest accuracy. GlobalAveragePooling2D was applied and a final layer was added with a Sigmoid activation function.

## Training, Testing, and Evaluation
A test accuracy of 93% was reached.

![download](https://github.com/sottohy/Sperm-Embryo-classification-models/assets/91037437/fd2ab9b1-ec28-4b38-9521-81500545c885)


![download (1)](https://github.com/sottohy/Sperm-Embryo-classification-models/assets/91037437/d6929596-e0bc-42bc-ac46-82abec262f46)

## Demo of the website (Under development)
![Screenshot (2421)](https://github.com/sottohy/Sperm-Embryo-classification-models/assets/91037437/fca48d40-d2ed-4e2b-b0e3-0029d4fb2165)

![Screenshot (2423)](https://github.com/sottohy/Sperm-Embryo-classification-models/assets/91037437/875fb5a0-41a4-4cae-a787-476bdedcfce3)




