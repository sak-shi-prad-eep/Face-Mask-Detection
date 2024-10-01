# Face Mask Detection Project

## Problem Statement
The COVID-19 pandemic has made face masks an essential part of public health measures. To assist in monitoring and enforcing mask-wearing policies, this project aims to develop an automated system that can classify whether an individual in an image is wearing a face mask or not.

## Data
The dataset used is the "Face Mask Dataset" from Kaggle, which includes:
- Total images: 7,553
- With mask images: 3,725
- Without mask images: 3,828
- Image dimensions: 128x128 pixels
- Attributes: RGB color channels

## Exploratory Data Analysis (EDA)
- **Data Distribution**: Analyzed the balance between mask and no-mask images.
- **Image Visualization**: Displayed sample images from both classes to understand the dataset.
- **Color Channel Analysis**: Explored the distribution of pixel values across RGB channels.

## Data Preprocessing
- **Resizing**: All images resized to 128x128 pixels for consistency.
- **Normalization**: Pixel values scaled to range [0, 1].
- **Augmentation**: Applied data augmentation techniques to increase dataset diversity.
- **Splitting**: Data split into training (80%) and test (20%) sets.

## Models
### Convolutional Neural Network (CNN)
- **Architecture**: Multiple convolutional and pooling layers, followed by dense layers.
- **Accuracy on Training Data**: 99.69%
- **Accuracy on Test Data**: 93.91%
- **Key Metrics**: Loss, Accuracy

## Results
- **Learning Curves**: Plotted training and validation accuracy/loss over epochs.
- **Confusion Matrix**: Visualized model performance on test set.
- **Sample Predictions**: Demonstrated model predictions on new images.

## Additional Insights
- Percentage of correct mask detections in test set: Approximately 93.91%
- Model performance on different types of masks (surgical, cloth, N95) could be an area for further investigation.

## Conclusion
The CNN model achieved high accuracy in detecting face masks, demonstrating its potential for real-world applications in public health and safety monitoring. Future work could focus on improving model generalization and real-time detection capabilities.
