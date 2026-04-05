Pneumonia Detection using CNN
📌 Problem Statement

The goal of this project is to develop a Convolutional Neural Network (CNN) model to classify chest X-ray images into two categories:

Pneumonia
Normal

The dataset consists of 5,863 JPEG images organized into three folders: train, test, and val.

📂 Dataset Description
Source: Pediatric chest X-ray images
Categories: Binary (Pneumonia / Normal)
Structure:
train/
   pneumonia/
   normal/
val/
   pneumonia/
   normal/
test/
   pneumonia/
   normal/
⚙️ Methodology
1. Data Preprocessing
Images resized to 150×150 pixels
Pixel values normalized (rescaled to [0,1])
Data augmentation applied:
Rotation
Zoom
Horizontal flipping
2. Model Architecture

A Convolutional Neural Network (CNN) was built with:

3 Convolutional layers (ReLU activation)
MaxPooling layers for downsampling
Flatten layer
Fully connected Dense layer
Dropout (0.5) to prevent overfitting
Output layer with Sigmoid activation
3. Training
Loss Function: Binary Crossentropy
Optimizer: Adam
Callback: EarlyStopping (to avoid overfitting)
Epochs: 15
4. Evaluation
Model evaluated using test dataset
Metric used: Accuracy
📊 Results
The model successfully classified X-ray images into Pneumonia and Normal categories.
Achieved good accuracy on test data (depends on training run).
EarlyStopping helped in preventing overfitting.
🚧 Challenges Faced
Handling dataset structure after unzipping
Presence of unnecessary _MACOSX folder
Ensuring correct directory paths in Google Colab
✅ Conclusion

The CNN model demonstrated effective performance in classifying chest X-ray images. With further improvements such as transfer learning (e.g., ResNet50), accuracy can be significantly enhanced.

🚀 Future Improvements
Use pre-trained models (Transfer Learning)
Hyperparameter tuning
Add confusion matrix and ROC curve
Increase dataset size
🛠️ Tools & Technologies
Python
TensorFlow / Keras
Google Colab
NumPy, Matplotlib
