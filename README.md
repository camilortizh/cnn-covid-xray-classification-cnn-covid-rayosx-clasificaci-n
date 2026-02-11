# CNN para la detección de COVID-19 en radiografías de tórax

## Descripción general
Este proyecto implementa una Red Neuronal Convolucional (CNN) para clasificar imágenes de radiografías de tórax en dos categorías:
- Normal  
- COVID-19  

El objetivo es construir un modelo de aprendizaje profundo capaz de detectar enfermedades pulmonares a partir de imágenes médicas.

## Conjunto de datos
Conjuntos de datos utilizados:
- COVID-19 Radiography Database (Kaggle)  
- Chest X-ray Images (Pneumonia)  

Las imágenes fueron redimensionadas a 200x200 píxeles y convertidas a escala de grises.

## Preprocesamiento de datos
- Eliminación de archivos innecesarios  
- Conversión a escala de grises  
- Redimensionamiento de imágenes (200x200)  
- Normalización de píxeles (0-255 → 0-1)  
- Aumento de datos (rotaciones, desplazamientos y cambios de brillo)  
- Balanceo de clases  
- Codificación One-Hot  
- División en entrenamiento y prueba (80/20)  

## Arquitectura del modelo
- CNN secuencial  
- Capas convolucionales con tamaño de kernel 5  
- Capas de MaxPooling  
- Dropout (40%)  
- Capa totalmente conectada (200 neuronas)  
- Capa de salida con activación sigmoide (clasificación binaria)  

Total de parámetros entrenables: 2,839,258  

## Entrenamiento
- Optimizador: Adam  
- Tasa de aprendizaje: 0.01  
- Métricas: Exactitud (Accuracy) y Precisión  

## Resultados
- Exactitud en entrenamiento: 92.7%  
- Exactitud en validación: 93.3%  
- Exactitud en prueba: 91.5%  
- Precisión en prueba: 89.0%  

El modelo muestra buena capacidad de generalización sin sobreajuste significativo.

## Conclusiones
El modelo CNN logró un alto rendimiento manteniendo eficiencia computacional. Futuras mejoras podrían incluir:
- Arquitectura más profunda  
- Transfer learning  
- Ajuste de hiperparámetros  

## Autores
- Camilo Ortiz  
- Santiago Forero  
- Julián Páez  

Pontificia Universidad Javeriana  
Bogotá, Colombia  

---

# CNN for COVID-19 Detection from Chest X-Rays

## Overview
This project implements a Convolutional Neural Network (CNN) to classify chest X-ray images into two categories:
- Normal  
- COVID-19  

The goal is to build a deep learning model capable of detecting pulmonary diseases from medical imaging data.

## Dataset
Datasets used:
- COVID-19 Radiography Database (Kaggle)  
- Chest X-ray Images (Pneumonia)  

Images were resized to 200x200 pixels and converted to grayscale.

## Data Preprocessing
- Removal of unnecessary files  
- Grayscale conversion  
- Image resizing (200x200)  
- Pixel normalization (0-255 → 0-1)  
- Data augmentation (rotations, shifts, brightness changes)  
- Class balancing  
- One-hot encoding  
- Train/Test split (80/20)  

## Model Architecture
- Sequential CNN  
- Convolutional layers with kernel size 5  
- MaxPooling layers  
- Dropout (40%)  
- Fully connected layer (200 neurons)  
- Output layer with sigmoid activation (binary classification)  

Total trainable parameters: 2,839,258  

## Training
- Optimizer: Adam  
- Learning rate: 0.01  
- Metrics: Accuracy and Precision  

## Results
- Training accuracy: 92.7%  
- Validation accuracy: 93.3%  
- Test accuracy: 91.5%  
- Test precision: 89.0%  

The model shows good generalization without significant overfitting.

## Conclusions
The CNN model achieved strong performance while maintaining computational efficiency. Future improvements could include:
- Deeper architecture  
- Transfer learning  
- Hyperparameter tuning  

## Authors
- Camilo Ortiz  
- Santiago Forero  
- Julián Páez  

Pontificia Universidad Javeriana  
Bogotá, Colombia  


