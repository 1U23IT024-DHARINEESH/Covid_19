# Covid_19
# COVID-19 Image Classification

This project classifies medical images into COVID and Normal categories using Convolutional Neural Networks (CNN). It uses image preprocessing and Deep Learning techniques to identify patterns in the images.

## Business Objective

COVID-19 screening can benefit from tools that help analyze medical images consistently. This project explores CNN-based image classification to distinguish COVID-labeled images from Normal-labeled images.

## Dataset Features

The dataset includes:

- Total Images: 251
- COVID Images: 111
- Normal Images: 140
- Image Size: 128 × 128 pixels
- Color Channels: 3 (RGB)

## Data Preprocessing

The project includes:

- Loading images from a NumPy file.
- Loading labels from a CSV file.
- Checking image and label dimensions.
- Encoding image labels using Label Encoder.
- Normalizing pixel values.
- Stratified train-validation-test splitting.

The data is divided into:

- 70% Training Data (175 images)
- 15% Validation Data (38 images)
- 15% Testing Data (38 images)

## Deep Learning Models

Two CNN architectures are compared:

1. **CNN Model 1:** Three Convolutional Layers with Max Pooling and Dense Layers.
2. **CNN Model 2:** Two Convolutional Layers with Max Pooling and additional Dense Layers.

Both models use:
- Adam Optimizer
- Binary Crossentropy Loss
- ReLU Activation
- Sigmoid Output
- 10 Epochs
- Batch Size: 8

## Evaluation Metrics

The models are evaluated using:

- Training Accuracy
- Validation Accuracy
- COVID Recall
- Test Accuracy
- Test COVID Recall

COVID Recall is important because it measures how many actual COVID-labeled images are correctly identified by the model.

## Final Result

Both CNN models achieve the following validation results:

- Training Accuracy: `1.000`
- Validation Accuracy: `0.9737`
- COVID Recall: `1.000`

Final test performance of CNN Model 2:

- Test Accuracy: `1.000`
- Test COVID Recall: `1.000`

These results are based on the available dataset and test split. Further validation on larger, independent datasets is required before any real-world use.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- TensorFlow
- Keras
- Scikit-learn
- Jupyter Notebook

## Conclusion

This project demonstrates the use of CNN architectures for COVID-19 image classification. Two CNN models are trained and compared using accuracy and COVID Recall. Both models achieved 97.37% validation accuracy, while the second model achieved 100% test accuracy on the available test dataset.

**Note:** This is an educational project, not a substitute for professional medical diagnosis.
