# Musical Instrument Classification  

This project aims to classify **10 different musical instruments** using Deep Learning, exploring two approaches:  
- Custom Convolutional Neural Network (CNN)  
- Transfer Learning with MobileNetV2  

---

## Introduction  

Identifying musical instruments from images is a challenging machine learning problem. This project investigates two approaches:  
- Training a CNN from scratch  
- Using MobileNetV2 for transfer learning, leveraging pre-trained weights for better generalization.  

---

## Instruments Classified  

The dataset includes the following 10 instruments:  

- Accordion  
- Banjo  
- Drum  
- Flute  
- Guitar  
- Harmonica  
- Saxophone  
- Sitar  
- Tabla  
- Violin  

---

## Methodology  

### CNN Model  
- A custom Convolutional Neural Network was built from scratch.  
- Includes convolutional layers, pooling layers, and fully connected layers.  
- Learns features hierarchically from raw image data.  

### Transfer Learning with MobileNetV2  
- Used MobileNetV2 pre-trained on ImageNet.  
- Fine-tuned final layers on the instrument dataset.  
- Beneficial for small datasets, enabling faster convergence and better performance.  

---

## Performance  

| Model                         | Training Accuracy | Validation Accuracy |  
|-------------------------------|-------------------|---------------------|  
| Custom CNN                     | 0.6875            | 0.5483              |  
| Transfer Learning (MobileNetV2) | 0.625             | 0.7557              |  

### Observations  
- MobileNetV2 achieved significantly better validation accuracy.  
- The custom CNN overfit slightly (training > validation accuracy).  
- Transfer learning generalized better despite lower training accuracy.  

---

## Dependencies  

- scikit-learn → Accuracy score, confusion matrix  
- tensorflow → Deep learning framework  
- tensorflow.keras → High-level API for model building  
- ImageDataGenerator → Real-time data augmentation  
- MobileNetV2 → Pre-trained transfer learning model  

---
Author: Surrabhi Pandey

