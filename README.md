Freiburg Grocery Images Classification
This project focuses on classifying images from the Freiburg Grocery Images dataset using different deep learning models. The models compared in this study include Convolutional Neural Networks (CNN), Multi-Layer Perceptrons (MLP), and Capsule Networks (CapsNet).


Authors:
Deniz Kaya

Levent Burcalıoğlu

Project Overview:
The objective of this project is to apply deep learning models to classify grocery items and compare the performance of these models. The dataset consists of grocery images in 25 classes, such as milk, oil, spices, and sugar. Each class contains no fewer than 97 images, totaling 4,947 images. The dataset was expanded to 25,000 images using data augmentation techniques to improve model performance.

Dataset:
Source: The Freiburg Grocery Images dataset is available for download here.
Image resolution: 256x256 pixels.
Class distribution: The dataset is imbalanced, with some classes having as few as 100 images, while others have more than 300.
Models Used:
MLP (Multi-Layer Perceptron)

Input: Grayscale images
Hidden Layers: 256, 128, 64, 32
Optimizer: Adam
Best performance: 52.94% training accuracy, 29.35% validation accuracy
CNN (Convolutional Neural Networks)

Three different CNN models were used, including AlexNet.
The best CNN model achieved 82.52% training accuracy and 70.48% validation accuracy with Adam optimizer and L2 regularization.
CapsNet (Capsule Networks)

Introduced to address limitations of CNNs, particularly in handling different perspectives of images.
Performance was lower than CNNs, but better at preserving spatial relationships in images.
Optimization & Regularization Techniques:
Optimizers used: Adam, RMSprop
Regularization techniques: Dropout, Early Stopping, Batch Normalization, Data Augmentation, L2 Regularization

Results:
MLP: Low accuracy, not well-suited for image classification tasks.
CNN: Achieved the best results, with models performing between 60% and 70% in terms of accuracy.
CapsNet: While CapsNet models are more complex and capable of handling image orientation, they did not outperform CNNs on this dataset.

Conclusion:
CNN models provided the highest classification accuracy for the Freiburg Grocery Images dataset. While CapsNet is promising for more complex tasks, it requires more computational resources and did not perform as well as CNNs for this dataset.

Requirements:
Python
TensorFlow or PyTorch
Freiburg Grocery Images dataset

How to Run:
Download the dataset from the link provided.
Install the required dependencies.
Run the training script for the models to reproduce the results.
