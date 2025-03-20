The system:

Identifies plant diseases from leaf images.
Supports multiple plant types, including:
Corn
Peach
Pepper
Potato
Soybean
Tomato
Generates evaluation reports with accuracy, precision, recall, F1-score, and a confusion matrix.


/Plant-Disease-Classification
├── /data
│   ├── /train         # Training dataset
│   └── /validation    # Validation dataset
├── /models
│   └── *.keras        # Saved models for each plant type
├── /code
│   ├── plant_disease_classifier.py  # Model training script
│   ├── evaluate.py                   # Model evaluation script
│   └── predict.py                    # Real-time prediction script
└── README.md


Features
Data Preprocessing with augmentation using ImageDataGenerator
CNN model with multiple convolution and pooling layers
Individual models trained for each plant type
Model evaluation and classification reports
Normalized confusion matrix for visual analysis

Model Architecture
Convolutional Layers: Feature extraction with ReLU activation.
Pooling Layers: Max pooling to reduce dimensionality.
Flatten Layer: Converts feature maps to a single vector.
Dense Layers: Fully connected layers for classification.
Dropout Layer: Prevents overfitting.


Dataset Description
Images of healthy and diseased leaves for each plant type.
Augmented with rotation, zoom, and flip for better model generalization.
