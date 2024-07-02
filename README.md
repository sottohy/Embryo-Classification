# Embryo Classification Model Using Transfer Learning

## Classification model for embryo images depending on the presence of blastocysts
## Link to the dataset: https://osf.io/3kc2d/

#### The motivation behind this project is to develop a model that aids in the IVF process by classifying embryo images as good or bad. The goodness or badnees of the images depend on whether the embryo is a blastocyst or not, respectively. The main idea of the project is to create a model designed for the selection phase in the IVF process. This model aims to improve the efficiency, precision, and success rates of IVF procedures by eliminating the human error factor.

## Preprocessing
The original data was classified into four folders, ED1, ED2, ED3, and ED4.

Folders ED1, ED2, and ED4 has 5 folders inside of them and use the 5-category system, where folders 1,2 refer to non-blastocysts and folders 3, 4, 5 refer to blastocysts.

The ED3 folder has 2 folders inside of it and use the 2-category system, where folder 1 refers to blastocysts and folder 2 refers to non-blastocysts.


## Model Selection & Architecture
The chosen model was ResNet101, as it was previously used in similar cases and resulted in the highest accuracy. 

## Training, Testing, and Evaluation
A test accuracy of 93% was reached.

![malak accuracy 93](https://github.com/sottohy/Embryo-Classification/assets/91037437/e9c347fa-2507-48f2-bdff-60ade59ae6d3)

![malak cm 93](https://github.com/sottohy/Embryo-Classification/assets/91037437/c22c6efa-bd88-48b8-ac92-df85c42fde4c)

## Demo of the website (Under development)
![Screenshot (2584)](https://github.com/sottohy/Embryo-Classification/assets/91037437/8e65a352-c04f-426c-ab87-67f2e4067442)

![Screenshot (2585)](https://github.com/sottohy/Embryo-Classification/assets/91037437/268a591f-561b-4a1e-8e14-3996342992b2)



