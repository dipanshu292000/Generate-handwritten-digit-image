Plant Disease Classification Using InceptionV3

This project implements a plant disease classification model using the InceptionV3 architecture. 
The model is designed to classify various plant diseases based on leaf images from the PlantVillage dataset. 
The use of the InceptionV3 model allows for high accuracy and efficient feature extraction from images.

Dataset

Dataset Source:

-The PlantVillage dataset is used, containing images of healthy and diseased plant leaves across 38 classes.

Number of Classes: 

-38 different classes, each representing a specific plant disease or a healthy plant condition.

Dataset Structure: 

-The dataset is organized into folders representing different classes.

Project Workflow

Data Preparation:

-The dataset is downloaded from Kaggle and extracted into the appropriate directory structure.
-Image data is preprocessed using TensorFlow's ImageDataGenerator for augmentation and rescaling.

Model Architecture:

Base Model:

-InceptionV3 with pre-trained weights from ImageNet, excluding the top layers.

Custom Layers: 

-Additional fully connected layers are added on top of the InceptionV3 model to adapt it for the plant disease classification task.

Training:

-The model is compiled using the Adam optimizer and categorical cross-entropy loss.
-Training is conducted with early stopping and model checkpoint callbacks to save the best-performing model and prevent overfitting.

Evaluation:

-The trained model is evaluated on a validation set, and accuracy is reported.
-The best model is saved in the .keras format for future inference.
