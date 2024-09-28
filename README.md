# Project Background
### Overview
Brain tumors are life-threatening and require early, accurate diagnosis to improve patient outcomes. Manual analysis of MRI scans can be time-consuming and prone to human error. To address this, we developed a deep learning-based classifier using Convolutional Neural Networks (CNNs) to automatically detect brain tumors from MRI images. Our goal is to provide a fast and reliable tool that assists healthcare professionals in diagnosis through a web-based application built with Flask.

### Objectives
- Build a CNN model to classify brain tumors as benign or malignant.
- Integrate the model into a Flask-based web application for real-time image uploads and predictions.
- Ensure the interface is user-friendly for medical professionals to easily interpret results.

### Tools and Technologies
- **Deep Learning:** TensorFlow/Keras for model training.
- **Web Framework:** Flask for the backend.
- **Frontend:** HTML, CSS, JavaScript for the user interface.

This project enhances diagnostic efficiency and accuracy in healthcare by providing an automated, accessible tool for brain tumor detection. The solution is scalable, adaptable, and demonstrates the impact of AI in medical imaging.

# Summary
### Overview
This project aimed to create a brain tumor classification system using deep learning, specifically focusing on MRI image analysis. A Convolutional Neural Network (CNN) was developed and integrated into a Flask-based web application, allowing users to upload MRI scans and receive real-time predictions. The project’s goal was to assist medical professionals by providing an automated tool for detecting brain tumors, improving diagnostic efficiency.

### Key Results
- **Model Accuracy:** The classifier achieved an accuracy of 81.29% on the test dataset.
- **Optimizer & Learning Rate:** The model was trained using the Adam optimizer with an initial learning rate of 0.001, which was dynamically reduced to 0.0005 using the **ReduceLROnPlateau** callback.
- **Callbacks:** In addition to ReduceLROnPlateau, the training process utilized **EarlyStopping** to prevent overfitting by halting training when validation loss stopped improving, and **ModelCheckpoint** to save the best model weights during training.
- **Data Augmentation:** Applied various data augmentation techniques (e.g., rotation, zooming, flipping) to enhance generalization and reduce overfitting.
- **Freezing and Unfreezing Layers:** Experimented with freezing and unfreezing layers of the neural network, but observed no significant performance improvements.

### Challenges and Next Steps
- **Limited Progress with Layer Freezing:** Freezing and unfreezing certain layers showed no noticeable improvements, suggesting that fine-tuning may need further exploration.
- **Next Steps:**
- **Hyperparameter Tuning:** Optimize learning rates, batch sizes, and dropout rates.
- **Optimizer Tuning:** Consider trying different optimizers such as SGD with momentum or RMSprop to see if performance improves.
- **Learning Rate Schedulers:** Experiment with more dynamic learning rate schedules (e.g., Cyclical Learning Rates) for potential gains.
- **Increase Model Complexity:** Try deeper architectures or transfer learning from pre-trained models like ResNet or Inception for improved feature extraction.
