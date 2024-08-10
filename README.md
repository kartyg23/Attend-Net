# Automated Attendance System with Facial Recognition

## Overview
This project presents a comprehensive automated attendance system that leverages facial recognition technology. It utilizes Haar Cascade, MTCNN, and FaceNet for detecting and recognizing faces. The application is hosted on Huggingface Spaces and provides an interactive interface through Gradio.

## Demo
Check out the live demo of the automated attendance system [here](https://huggingface.co/spaces/pranav-5644/automated_attendance_using_facenet).
We have also provided some examples in demo for testing.

## Installation

**Clone the repository :**
   ```bash
   git clone https://github.com/kartyg23/Attend-Net.git
   cd Attend-Net
   ```
**Install the required packages :**
   ```bash
    pip install -r requirements.txt
   ```
**Ensure you are using Python 3.6 or higher.**

## Workflow and File Structure

1. **[Face_detection](Face_detection.ipynb) :** The system uses Haar Cascade and MTCNN to detect faces in from uploaded image.
2. **[Processing](Processing.ipynb) :** Process the images(one for each individual) in training_images folder to generate the embeddings for the siamese network.
3. **[data_processed](data_processed.pkl) :** stores the vector embeddings.
4. **[test_data](test_data.ipynb) :** evaluate the model on test_images using precision, recall , f1_score and plot a confusion matrix to get and idea of classification capabilities.
5. **[attendance](attendance.ipynb) :** use the vector embeddings to recognize faces stored in attendance_class folder and generate a text file for attendance.
6. **'class_attendance.jpg' :** name for input file.


## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.
