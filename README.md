# Live-Face-Detection-System
A Python project that performs real-time face detection using OpenCV’s Haar Cascade Classifier and webcam feed.

# Face Detection using OpenCV

## Description

This project demonstrates **real-time face detection** using OpenCV’s Haar Cascade Classifier.
The application captures video from your webcam, detects faces in each frame, and highlights them with a green rectangle.

---

## Features

* Real-time face detection using the webcam.
* Uses Haar Cascade Classifier for fast and accurate detection.
* Displays live video with detected faces outlined.
* Press `'a'` to exit the application.

---

## Requirements

* Python 3.13 (or compatible)
* OpenCV (`opencv-python`)
  Install via pip:

  ```bash
  pip install opencv-python
  ```

---

## File Structure

```
face_detection/
│
├── face_detection.py      # Main Python script
├── README.md              # Project documentation
└── haarcascade_frontalface_default.xml  # Haar cascade XML file (provided by OpenCV)
```

---

## Usage

1. Clone or download this repository.
2. Ensure OpenCV is installed:

   ```bash
   pip install opencv-python
   ```
3. Run the Python script:

   ```bash
   python face_detection.py
   ```
4. A window will open showing live webcam video.
5. Detected faces will be outlined in green rectangles.
6. Press `'a'` to exit the application.

---

## Notes

* Make sure the path to `haarcascade_frontalface_default.xml` is correct.
* You can find the Haar cascades in OpenCV’s data directory:

  ```python
  import cv2
  print(cv2.data.haarcascades)
  ```
* Adjust `scaleFactor` and `minNeighbors` in `detectMultiScale` for better detection accuracy.

---

## License

This project is open-source and free to use for educational purposes.

---

