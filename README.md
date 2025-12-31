 DermalScan – Skin Aging Detection System
 Project Overview

DermalScan is an AI-based skin aging detection system developed as part of the Infosys Springboard Internship.
The project uses deep learning to analyze facial images and classify skin conditions such as:

Wrinkles

Dark Spots

Puffy Eyes

Clear Skin

The system supports single face and group photo analysis, detects multiple faces, and displays predictions with confidence scores through a web-based UI.

 Objectives

To build a CNN-based model for skin condition classification

To preprocess and augment facial image datasets

To detect faces from uploaded images

To classify skin aging conditions using a trained model

To present results through a simple and interactive Web UI

 Technologies Used

Python

TensorFlow / Keras

OpenCV

MTCNN (Face Detection)

Gradio (Web UI)

Google Colab

NumPy, Pandas

📂 Dataset Structure

The dataset is organized into four classes, each containing facial images:

dataset/
│
├── wrinkles/
├── dark_spots/
├── puffy_eyes/
└── clear_skin/


Each folder contains approximately 50 images

Images were resized to 224×224

Dataset was normalized and augmented

⚙️ Methodology
🔹 Image Preprocessing

Image resizing to 224×224

Normalization (pixel values scaled between 0–1)

Data augmentation (rotation, zoom, flip)

🔹 Model Training

CNN-based deep learning model trained in Google Colab

Model trained using labeled dataset folders

Output saved as DermalScan_Model.h5

🔹 Face Detection

MTCNN used to detect faces from both single and group images

Each detected face is cropped and passed to the model for prediction

🔹 Classification

Model predicts one of the four skin conditions

Confidence score calculated for each prediction

🌐 Web UI (Milestone 4)

Web UI implemented using Gradio

Allows image upload (single or group photo)

Displays:

Original image

Annotated image with bounding boxes

Predicted label for each detected face

Confidence percentage

Prediction results table

Generates a downloadable CSV report containing:

Image name

Predicted condition

Confidence

Timestamp

 Output Example

Green bounding box drawn around detected faces

Label (e.g., dark_spots) and confidence displayed

CSV report generated for record and analysis

 Limitations

Model performance depends heavily on dataset quality

Some class imbalance may affect prediction accuracy

Limited dataset size impacts generalization

 Future Enhancements

Improve dataset quality and balance

Train with larger and more diverse facial datasets

Improve accuracy for fine-grained skin condition detection

Deploy as a cloud-hosted web application

 Conclusion

The DermalScan project successfully demonstrates the use of deep learning and computer vision techniques to detect and classify skin aging conditions.
It integrates preprocessing, model training, face detection, and web deployment into a complete AI pipeline suitable for real-world applications.

👨‍💻 Developed By

Manda Sasank
B.Tech – Computer Science & Engineering
Infosys Springboard Internship
