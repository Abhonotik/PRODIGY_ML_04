🤖 Hand Gesture Recognition System using CNN & OpenCV
This project implements a real-time hand gesture recognition system using deep learning. The system classifies hand gestures from video frames and can be used to control applications through simple gestures — paving the way for intuitive Human-Computer Interaction (HCI).

📁 Dataset
LeapGestRecog Dataset

10 gesture classes

40,000+ grayscale images

Captured using a Leap Motion controller

Image format: .png

Image size: 320x240 (resized to 64x64 during preprocessing)

🧠 Model Architecture
Built using TensorFlow/Keras, the CNN model includes:

Conv2D layers for feature extraction

MaxPooling for spatial reduction

Flatten + Dense layers for classification

Dropout to reduce overfitting

Achieved ~100% accuracy on the validation and test datasets. 🏆

📸 Real-Time Detection
Using OpenCV, the trained model performs gesture classification from webcam input in real time.

How it works:
Captures video frames

Detects and crops the region of interest (ROI)

Converts to grayscale and resizes to 64x64

Predicts the gesture class using the trained CNN model

Displays the predicted gesture on the video stream

🧪 Project Structure
bash
Copy
Edit
├── dataset_loader.py       # Loads and preprocesses LeapGestRecog dataset
├── train_model.py          # Builds, trains, and saves the CNN model
├── gesture_recognition.py  # Real-time webcam-based gesture prediction
├── model.h5                # Trained model file
├── README.md               # Project documentation
