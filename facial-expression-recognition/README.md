# Facial Expression Recognition w/ Keras

Built and trained a convolutional neural network (CNN) in Keras to recognize facial expressions. The data consists of 48x48 pixel grayscale images of faces. The objective was to classify each face based on the emotion shown in the facial expression into one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral). OpenCV was used to automatically detect faces in images and draw bounding boxes around them. Once the model has been trained, saved, and exported the CNN, the trained model predictions was served to a web interface to perform real-time facial expression recognition on video and image data.

## Project Overview
### 1. Exploring the Dataset
- Display some images from every expression type in the Emotion FER dataset.
- Check for class imbalance problems in the training data.

### 2. Generate Training and Validation Batches
- Generate batches of tensor image data with real-time data augmentation.
- Specify paths to training and validation image directories and generates batches of augmented data.

### 3. Create a Convolutional Neural Network (CNN) Model
- Design a convolutional neural network with 4 convolution layers and 2 fully connected layers to predict 7 types of facial expressions.
- Use Adam as the optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.

### 4. Train and Evaluate Model
- Train the CNN by invoking the model.fit() method.
- Use ModelCheckpoint() to save the weights associated with the higher validation accuracy.
- Observe live training loss and accuracy plots in Jupyter Notebook for Keras

### 5. Save and Serialize Model as JSON String
- Use to_json(), which uses a JSON string, to store the model architecture.

### 6. Create a Flask App to Serve Predictions
- Use open-source code from "Video Streaming with Flask Example" to create a flask app to serve the model's prediction images directly to a web interface.

### 7. Create a Class to Output Model Predictions
- Create a FacialExpressionModel class to load the model from the JSON file, load the trained weights into the model, and predict facial expressions.

### 8. Design an HTML Template for the Flask App
- Design a basic template in HTML to create the layout for the Flask app.

### 9. Use Model to Recognize Facial Expressions in Videos
- Run the main.py script to create the Flask app and serve the model's predictions to a web interface.
- Apply the model to saved videos on disk.
