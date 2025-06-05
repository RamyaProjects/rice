# Rice Grain Classification with Convolutional Neural Networks (CNN)

**Overview**

This project implements a Convolutional Neural Network (CNN) to classify images of rice grains into five distinct varieties: Arborio, Basmati, Jasmine, Ipsala, and Karacadag. Utilizing TensorFlow and Keras, the model achieves high accuracy in distinguishing between these rice types, demonstrating the power of deep learning in agricultural applications.

**Dataset**

The dataset comprises 75,000 images, equally distributed among the five rice varieties. The images are organized in directories corresponding to each class:

rice_data/

  ├── Arborio/

  ├── Basmati/

  ├── Ipsala/

  ├── Jasmine/

  └── Karacadag/

**Requirements**
Before running the project, install the necessary dependencies:

```pip install tensorflow numpy pandas matplotlib seaborn scikit-learn```

**Results**

- Training Accuracy: 100%-

- Validation Accuracy: 100%

- Test Accuracy: 100%

The trained CNN model achieves an accuracy of 100% on the test set, demonstrating its effectiveness in classifying rice grain varieties. Detailed metrics such as precision, recall, and F1-score are also reported for each class.

**Model Architecture**

The CNN model consists of:

- **Convolutional Layers:** Extract features from input images.

- **Batch Normalization:** Stabilize and accelerate training.

- **MaxPooling Layers:** Reduce spatial dimensions.

- **Fully Connected Layers:** Perform classification.

- **Output Layer:** Softmax activation for multi-class classification.

**Callbacks Used:**

- **ModelCheckpoint:** Saves the model after each epoch.

- **ReduceLROnPlateau:** Reduces learning rate if validation loss plateaus.

- **EarlyStopping:** Stops training if validation loss doesn't improve.
