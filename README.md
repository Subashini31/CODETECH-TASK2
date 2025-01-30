# 🧠 Plant Disease Classification using CNN
 
This project focuses on classifying plant diseases using a **Convolutional Neural Network (CNN)** built with **Keras and TensorFlow**. The model is trained on a dataset of plant images and predicts the disease category based on image inputs.   🚀  
 
 ---

 ## Dataset  
- The dataset contains images of **38 different plant disease categories**.  
- Images are stored in appropriate folders for training and validation.  
 
## **🛠 Features**  

✔ **Convolutional Layers** – Extract spatial features from images  
✔ **Batch Normalization** – Speeds up training and stabilizes learning  
✔ **MaxPooling** – Reduces dimensionality and enhances feature extraction  
✔ **Global Average Pooling** – Reduces parameters and prevents overfitting  
✔ **Dropout Regularization** – Helps mitigate overfitting  
✔ **Adam Optimizer** – Ensures efficient training  
✔ **Learning Rate Scheduler** – Dynamically adjusts learning rate  
✔ **Data Augmentation** – Enhances dataset generalization  

---

## **🚀 Model Architecture**  

The CNN consists of **four convolutional blocks**, followed by **Global Average Pooling and Fully Connected Layers**:  

| Layer Type              | Output Shape      | Parameters |
|-------------------------|------------------|------------|
| Conv2D (32 filters)     | (256, 256, 32)   | 896        |
| BatchNormalization      | (256, 256, 32)   | 128        |
| MaxPooling2D           | (128, 128, 32)   | 0          |
| Conv2D (64 filters)     | (128, 128, 64)   | 18,496     |
| BatchNormalization      | (128, 128, 64)   | 256        |
| MaxPooling2D           | (64, 64, 64)     | 0          |
| Conv2D (128 filters)    | (64, 64, 128)    | 73,856     |
| BatchNormalization      | (64, 64, 128)    | 512        |
| MaxPooling2D           | (32, 32, 128)    | 0          |
| Conv2D (256 filters)    | (32, 32, 256)    | 295,168    |
| BatchNormalization      | (32, 32, 256)    | 1,024      |
| MaxPooling2D           | (16, 16, 256)    | 0          |
| GlobalAveragePooling2D | (256)            | 0          |
| Dense (256 neurons)    | (256)            | 65,792     |
| Dropout (0.5)          | (256)            | 0          |
| Dense (38 classes)     | (38)             | 9,766      |

---

## Performance  
- The model achieves good accuracy in classifying plant diseases.  
- The results can be further improved using data augmentation and fine-tuning.  
- Train Accuracy  : 98.47 %
- Test Accuracy   : 97.72 %
- Precision Score : 97.72 %
- Recall Score    : 97.72 %  





