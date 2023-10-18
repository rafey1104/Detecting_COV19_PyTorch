# Detecting COVID19 Using PyTorch 

## Problem Statement 
The project aims to create a machine learning model for classifying Chest X-ray images into three categories: Normal, Viral Pneumonia, and COVID-19. The objective was to assist in the early diagnosis of COVID-19 by leveraging deep learning techniques and a dataset from the [COVID-19 Radiography Database](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database) on Kaggle.


## Action 
-<h3>Dataset Preparation</h3>
 - The COVID-19 Radiography Database was used, containing images from the three categories: Normal, Viral Pneumonia, and COVID-19. 
 - A custom dataset was created to load and preprocess these images.
 - Training and test sets were prepared by splitting the data into these two sets, ensuring a balanced distribution of images.

-<h3>Image Transformations</h3>
 - Image transformations were defined to standardize the input data, including resizing, data augmentation (e.g., horizontal flipping), and normalization.

-<h3>Model Creation</h3>
 - A pre-trained ResNet-18 model from PyTorch's torchvision library was used.
 - The final fully connected layer of the model was replaced to match the three output classes (Normal, Viral Pneumonia, and COVID-19).

-<h3>Training the Model</h3>
 - The model was trained for a specified number of epochs using an Adam optimizer and cross-entropy loss.
 - The training loop includes evaluating the model's performance on the test set at regular intervals.
 - Training was stopped when the model achieved a satisfactory accuracy of 95% or more on the test set.


## Result
- The model was trained for one epoch, and the following results were achieved:
  - Training Loss: 0.1394
  - Validation Loss: 0.1394
  - Final Accuracy on the test set: 95.56%

