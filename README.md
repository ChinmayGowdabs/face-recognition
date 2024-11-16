# **Face Recognition and Attendance System**

This project implements a real-time **Face Recognition and Attendance System** using Python. It leverages machine learning (K-Nearest Neighbors) and computer vision (OpenCV) techniques to recognize faces from a webcam and record attendance in a CSV file.

---

## **Objective**

The main goal of this project is to create a system that:
1. Recognizes faces in real-time using a webcam.
2. Matches the detected faces with pre-trained data.
3. Records attendance along with timestamps in a CSV file.

---

## **Features**
- **Real-time Face Detection**: Detects faces in a video feed using Haar Cascade Classifier.
- **Face Recognition**: Uses a K-Nearest Neighbors (KNN) classifier to identify faces.
- **Attendance Logging**: Automatically logs the attendance of recognized individuals in a CSV file with a timestamp.
- **Text-to-Speech Feedback**: Provides auditory feedback when attendance is successfully taken.
- **CSV-Based Attendance**: Saves attendance with names and timestamps in a structured CSV format.

---

## **Technologies Used**
- **Programming Language**: Python
- **Libraries**:
  - **OpenCV**: For real-time face detection and image processing.
  - **scikit-learn**: For implementing the KNN classifier to recognize faces.
  - **NumPy**: For numerical computations and image array handling.
  - **Pickle**: To save and load the trained face data and labels.
  - **CSV**: For logging attendance data.
  - **pywin32**: For providing text-to-speech feedback on successful attendance recording.
- **Hardware**: Webcam for capturing real-time video feed.

---

## **Directory Structure**
Ensure your project folder has the following structure:
```
├── data/
│   ├── faces_data.pkl
│   ├── names.pkl
│   ├── haarcascade_frontalface_default.xml
├── Attendance/
├── background.png
├── test.py
├── README.md
```
**User Controls**:
   - Press **`o`** to log attendance for recognized faces.
   - Press **`q`** to exit the program.

** The attendance will be saved in the `Attendance/` folder, with a new CSV file created every day:
   - The filename will be in the format `Attendance_<date>.csv` (e.g., `Attendance_16-11-2024.csv`).
   - The CSV file will have the following columns:
     ```
     NAME, TIME
     ```

---

## **Real-Life Applications**
- **Educational Institutions**: Automate attendance marking for students and faculty.
- **Offices**: Track employee attendance.
- **Event Management**: Monitor attendee participation at conferences and events.

---

## **Limitations**
1. The accuracy of face recognition may decrease if the training dataset is small or the environment has poor lighting.
2. The system may not perform well with occlusions (e.g., faces partially covered by objects).
3. Faces need to be pre-registered in the system for accurate recognition.

---

## **Acknowledgments**
- OpenCV for face detection and image processing.
- Scikit-learn for implementing machine learning models.
- Python community for their contributions and support.

---

Contact:- chinmaygowdabs@gmail.com
