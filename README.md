# Melanoma Detection using Custom CNN

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information
- This project aims to develop a custom Convolutional Neural Network (CNN) model for accurately detecting melanoma and other oncological diseases from skin images.
- The business problem addressed is the early detection of melanoma, which is crucial for improving prognosis and reducing mortality rates associated with skin cancer.
- The dataset consists of 2357 images of malignant and benign oncological diseases, sourced from the International Skin Imaging Collaboration (ISIC).

## Objective
By leveraging deep learning techniques and custom CNN models, this project aims to contribute to the early detection and diagnosis of melanoma, ultimately improving patient outcomes and reducing mortality rates associated with this deadly form of cancer.

## Data
- Dataset: [Skin Cancer Dataset](https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view?usp=sharing)
  - Description: The dataset consists of 2357 images of malignant and benign oncological diseases, sourced from the International Skin Imaging Collaboration (ISIC). Images are sorted into 9 subdirectories corresponding to different types of skin cancer.
  - Format: Images in JPG format
  - Usage: Used for training and testing the CNN model for melanoma detection.

## Project Pipeline
1. **Data Reading/Data Understanding:**
   - Define the paths for train and test images from the dataset.
   
2. **Dataset Creation:**
   - Create train and validation datasets from the train directory with a batch size of 32.
   - Resize images to 180x180 pixels.
   
3. **Dataset Visualization:**
   - Develop code to visualize one instance of all the nine classes present in the dataset.
   
4. **Model Building & Training:**
   - Construct a CNN model capable of accurately detecting the nine classes in the dataset.
   - Choose appropriate optimizer and loss function for model training.
   - Train the model for approximately 20 epochs.
   - Evaluate model performance and check for evidence of overfitting or underfitting.
   
5. **Data Augmentation:**
   - Implement data augmentation to address underfitting or overfitting issues.
   
6. **Model Building & Training on Augmented Data:**
   - Build and train the CNN model on augmented data.
   - Evaluate model performance and assess if earlier issues are resolved.
   
7. **Class Distribution Analysis:**
   - Examine the current class distribution in the training dataset.
   - Identify classes with the least number of samples and those dominating the data proportionately.
   
8. **Handling Class Imbalances:**
   - Rectify class imbalances present in the training dataset using the Augmentor library.
   
9. **Model Building & Training on Rectified Class Imbalance Data:**
   - Build and train the CNN model on the rectified class imbalance data.
   - Evaluate model performance and assess if issues identified earlier are resolved.


## Conclusions
- The custom CNN model achieved high accuracy in detecting melanoma and other oncological diseases.
- Data augmentation techniques effectively addressed issues of overfitting and underfitting, improving model generalization.
- Class distribution analysis revealed class imbalances, which were rectified using the Augmentor library, leading to improved model performance.
- The final model demonstrated robustness in detecting melanoma, contributing to early diagnosis and improved patient outcomes.

## Technologies Used
- TensorFlow - version 2.5  
- Matplotlib - version 3.4  
- NumPy - version 1.19  
- PIL (Python Imaging Library)  
- Pandas - version 1.2  
- Augmentor - version 0.2  


## Acknowledgements
- This project was inspired by the need for automated melanoma detection tools in the medical field.
- The dataset used in this project was sourced from the International Skin Imaging Collaboration (ISIC).
- Portions of the code and methodology were adapted from various TensorFlow tutorials and documentation.

## Contact
Created by [@poronita](https://github.com/poronita/) - feel free to contact me!

