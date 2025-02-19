# Object Localization using Deep Learning

This project implements object localization using deep learning techniques. The goal is to detect and predict the bounding box coordinates of an object within an image. 

## Features
- Uses Convolutional Neural Networks (CNN) for feature extraction.
- Predicts bounding box coordinates along with object classification.
- Trained on a dataset with labeled object positions.

## How It Works
1. **Data Preprocessing**:
   - Loads the dataset containing images and corresponding bounding box annotations.
   - Performs normalization and augmentation to improve generalization.
   - Images are resized and normalized to match the model input requirements.

2. **Model Architecture**:
   - A CNN-based model is used for both classification and localization.
   - The final layer outputs class probabilities and bounding box coordinates.
   - Fully connected layers are added for bounding box regression.

3. **Training**:
   - The model is trained using a loss function combining classification and localization losses.
   - Optimized with Adam optimizer and validated using a separate dataset.
   - Model is trained for multiple epochs with early stopping to prevent overfitting.

4. **Evaluation & Output**:
   - Computes Intersection over Union (IoU) to assess bounding box accuracy.
   - Visualizes results by overlaying predicted bounding boxes on images.
   - Bounding box coordinates are compared with ground truth for accuracy assessment.

## Output
- The model predicts an object's class and bounding box.
- Outputs visualizations with the predicted bounding box drawn on images.

