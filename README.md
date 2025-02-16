**Face Recognition and Attendance System**

**Overview**

This project implements a face recognition and attendance system using deep learning models. It extracts faces from group photos, converts them into embeddings using FaceNet, and compares them with stored embeddings to identify individuals and mark attendance.

**Features**

Detects faces in a group photo using MTCNN.

Extracts individual faces from the group photo.

Converts extracted faces into embeddings using FaceNet.

Compares embeddings with a predefined database of known individuals.

Determines if a person is present in the group photo based on a distance threshold.

Displays extracted faces and recognized individuals.

Prerequisites

Before running the project, ensure you have the following dependencies installed:

pip install numpy pandas matplotlib opencv-python tensorflow keras_facenet mtcnn

**Project Structure**

├── images/                # Directory containing individual images of known people
│   ├── galgadot.jpg
│   ├── jordana.jpg
│   ├── paulwalker.jpg
│   ├── rickyune.jpg
│   ├── rock.jpg
│   ├── vindiesel.jpg
├── group_photo.jpg        # Sample group photo for testing
├── face_recognition.py    # Main script containing the face recognition logic

**Dependencies**

NumPy: For numerical computations.

Pandas: For data handling.

Matplotlib: For image visualization.

OpenCV: For image processing.

TensorFlow: For deep learning model inference.

Keras-FaceNet: For face embedding generation.

MTCNN: For face detection.

**Limitations**

Accuracy depends on the quality of the images.

Faces must be clearly visible for effective recognition.

The model might misidentify individuals with similar facial features.
