# Lab Assignment 2 – Transfer Learning using Pretrained Model

## Course Information

**Course Name:** Deep Learning  
**Lab Assignment:** Lab Assignment 2  
**Topic:** Research Paper Implementation with Pre-trained Model  

---

## Student Details

**Student Name:** Parimal Ahire  
**PRN:** 202301040067  

## Group Members

- Parimal Ahire  
- Rajveersinh Kher  
- Mohit Patil  
- Atharva Suryawanshi  

---

## Research Paper Reference

**Title:** Multiple Classification of Flower Images Using Transfer Learning  
**Authors:** Emine Cengil, Ahmet Cinar  
**Year:** 2019  

**Citation (IEEE format):**

E. Cengil and A. Cinar, "Multiple Classification of Flower Images Using Transfer Learning," *2019 International Artificial Intelligence and Data Processing Symposium (IDAP)*, Malatya, Turkey, 2019, pp. 1–5.

The paper demonstrates the use of pretrained CNN models such as VGG16, ResNet and AlexNet for flower classification using transfer learning.

---

## Objective

The objective of this assignment is to:
- Study a research paper using pretrained CNN models
- Implement transfer learning using VGG16
- Fine-tune classification layers
- Evaluate performance using standard metrics

---

## Dataset Used

**Dataset:** Flowers Recognition Dataset  

**Source:**
https://www.kaggle.com/datasets/alxmamaev/flowers-recognition

**Classes:**
- Daisy
- Dandelion
- Rose
- Sunflower
- Tulip

The dataset is organized into class folders which makes it suitable for CNN classification.

---

## Implementation Steps

The following steps were implemented:

1. Dataset loading from Google Drive
2. Dataset preprocessing and visualization
3. Loading VGG16 pretrained model
4. Freezing convolution layers
5. Adding custom dense classifier layers
6. Model training
7. Model evaluation using performance metrics

---

## Model Details

**Pretrained Model:** VGG16  
**Framework:** TensorFlow / Keras  

Transfer learning approach:
- ImageNet pretrained weights used
- Convolution base frozen
- Custom dense layers added
- Only classifier layers trained

---

## Hyperparameters

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Batch Size | 32 |
| Image Size | 224×224 |
| Epochs | 10 |

---

## Results

**Training Accuracy:** 96.93%  
**Validation Accuracy:** 89.11%

Performance metrics:
- Precision: 0.89
- Recall: 0.89
- F1 Score: 0.89

The confusion matrix shows that most predictions are correct with minor misclassification between similar flower classes.

---

## Comparison with Research Paper

The research paper reports approximately 93% accuracy using VGG16, while the implemented model achieved about 89% validation accuracy. The small difference may be due to dataset differences and training parameters.

---

## Conclusion

Transfer learning using the VGG16 pretrained model achieved good classification accuracy with limited training data. The model obtained about 97% training accuracy and 89% validation accuracy, showing that pretrained CNN models can significantly reduce training effort while maintaining strong performance.

---

## Tools and Technologies

- Python
- TensorFlow
- Keras
- Google Colab
- NumPy
- Matplotlib
- Scikit-learn
