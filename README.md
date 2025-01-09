# CNN-based Algae Species Recognition for Hydrogen Production Project

## **Project Overview**

This project is part of a larger research initiative focused on **algae-based hydrogen production**. The primary objective is to develop a **Convolutional Neural Network (CNN)** model that can accurately classify algae species based on microscopic images. By identifying the species of algae, it is easier to understand their potential for hydrogen production, as different algae species exhibit varying efficiencies in the production of hydrogen.

The algae classification system is intended to support the overall hydrogen production research by enabling more efficient tracking, analysis, and experimentation with different algae species.

---

## **Project Aim**

The aim of this specific part of the project is to:
- **Develop an image classification model**.
- **Automate the algae classification process**.
- Serve as a component in a larger research project exploring the use of algae for clean hydrogen production.

### **Context: Hydrogen Production from Algae**
Algae, particularly certain species, can produce hydrogen gas (H₂) under specific conditions. This project aims to facilitate the study of algae by automating the classification of species, which can then be analyzed for their hydrogen production capabilities.

---

## **Approach**

### **Dataset**
The model uses the **Algae_Detection_Project** dataset, which contains images of various algae species. These images are labeled with their corresponding species and are used to train the model for classification tasks. The algae species identified can then be studied further for their **hydrogen production** potential.

- **Dataset Source:** [Algae Detection Project Dataset on Roboflow](https://universe.roboflow.com/training-gynfa/algae_detection_project-vyfu6)
  
This dataset contains **34 classes**, each representing a different algae species. These images are pre-processed, augmented, and split into training and validation datasets.

### **Model Architecture**
The image classification task is solved using a **Convolutional Neural Network (CNN)**, which is designed to automatically learn features from the raw image data. 

- **CNN Architecture**: The model consists of convolutional layers to extract features, max-pooling layers for dimensionality reduction, dropout layers to prevent overfitting, and dense layers for classification.
- **Data Augmentation**: The model employs data augmentation techniques like random flips, rotations, and zooms to increase the size and variability of the training dataset.

### **Training and Evaluation**
The model is trained using the **Adam optimizer** and **SparseCategoricalCrossentropy** loss function, with performance measured by **accuracy** on the validation set.

---

## **Key Results**

- **Final Training Accuracy**: 92.02%
- **Final Validation Accuracy**: 87.29%

The CNN model achieved a **92.02% training accuracy** and **87.29% validation accuracy**, demonstrating reliable performance in classifying algae species. While promising, the model is still a work in progress, with ongoing efforts to improve its generalization and robustness. It serves as a strong foundation for automating species identification.

### **Sample Prediction**
You can test the model by classifying new algae images. Here's an example of how to use the trained model for classification:

```python
classify_images('Samples/anabaenasample.jpg')
```

 ## **References**
1. Roboflow. (2024). *Algae_Detection_project Dataset*. Available at [Roboflow Universe](https://universe.roboflow.com/training-gynfa/algae_detection_project-vyfu6).  
   Citation: **Roboflow** (2024). "Algae_Detection_project Dataset". *Roboflow Universe*. Available online: [https://universe.roboflow.com/training-gynfa/algae_detection_project-vyfu6](https://universe.roboflow.com/training-gynfa/algae_detection_project-vyfu6).
