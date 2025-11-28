### Facial Emotion Recognition Project 😃🎥

A real-time Facial Emotion Recognition (FER) system using OpenCV, Keras,
and a pre-trained deep learning model. The system detects faces using Haarcascade
and predicts emotions based on the FER2013 dataset.

---

### 📑 Table of Contents
- Project Structure
- Requirements
- Dataset
- Training the Model
- Haarcascade for Face Detection
- Running Emotion Detection
- Features
- Example Output
- Notes

---

### 🏗 Project Structure

<img width="744" height="365" alt="image" src="https://github.com/user-attachments/assets/0cbd045a-7a52-4a6b-8420-93d50222ad4e" />




---

### ⚙️ Requirements
- **Python:** 3.10 recommended
- **Packages:**
  - numpy
  - opencv-python
  - keras
  - pillow
  - tensorflow

---

### 📂 Dataset
- Optional – only if you want to train the model yourself
- **Download link:** [FER2013 Dataset](https://www.kaggle.com/msambare/fer2013)
- **Location:** Place the CSV file inside the `data` folder: `data/fer2013.csv`

---

### Training the Model
-----------------
- Command to train: `python TrainEmotionDetector.py`
- Output files after training:
  - emotion_model.json → Model architecture
  - emotion_model.h5 → Model weights
- Move these files into the `model` folder

---

### Haarcascade for Face Detection
------------------------------
- The project uses Haarcascade classifier to detect faces before predicting emotions
- File: haarcascade_frontalface_default.xml
- Place this file inside the `model` folder

---

### Running Emotion Detection
------------------------
- Command: `python TestEmotionDetector.py`
- Description:
  Open the webcam or a video file, detect faces using Haarcascade,
  predict emotions using the trained model, and display rectangles
  around faces with predicted emotions above each face in real-time.

---

### Features
--------
- Real-time face detection with bounding boxes
- Predicts 7 basic emotions: Angry, Disgusted, Fearful, Happy, Neutral, Sad, Surprised
- Works with video files or live webcam feed
- Lightweight and efficient for real-time detection

---

### Example Output
--------------
- Faces are detected with rectangles
- Predicted emotions appear above each face in real-time
- Works smoothly with webcam or pre-recorded videos

---

### 🎥 Demo
<img width="1298" height="685" alt="image" src="https://github.com/user-attachments/assets/5591645a-05d0-4b2a-a347-a6d7aa5cb074" />

 

---

### Notes
-----
- Ensure the `model` folder contains: emotion_model.json, emotion_model.h5, and haarcascade_frontalface_default.xml
- For faster detection, reduce the resolution of video input or webcam feed
- Recommended to train the model on a GPU for faster performance if available










