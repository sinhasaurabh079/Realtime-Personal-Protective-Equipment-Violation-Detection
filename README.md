
# Real-time PPE Violation Detection System

This project aims to enhance safety standards on construction sites by detecting violations of Personal Protective Equipment (PPE) in real-time using computer vision and machine learning techniques.

## Features

- **Real-time Monitoring:** Continuously monitors video feeds for PPE violations.
- **High Accuracy Detection:** Utilizes the YOLOv7 model trained on PyTorch for accurate detection of PPE violations.
- **Automated Alerts:** Sends email notifications to authorities using the Gmail API upon detecting a violation.
- **Scalable Deployment:** Containerized using Docker and deployed on an NVIDIA DGX A100 server.

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Flask, PyTorch, YOLOv7
- **Dataset Preparation:** Roboflow
- **Notification System:** Gmail API
- **Containerization:** Docker
- **Deployment:** NVIDIA DGX A100 server

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/sinhasaurabh079/Realtime-Personal-Protective-Equipment-Violation-Detection.git
    cd Realtime-Personal-Protective-Equipment-Violation-Detection
    ```

2. **Set up the virtual environment:**
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

4. **Copy the Gmail API token in the folder and run send_mail.py:**
    ```sh
    python3 send_mail.py
    ```
5. **Run the program app.py for seeing:**
    ```sh
    python3 app.py
    ```


## Usage

1. **Prepare the dataset using Roboflow:**
    - Label the images for PPE detection.
    - Export the dataset in a format compatible with YOLOv7.
    - Place the dataset in the appropriate directory as specified in the project.

2. **Train the YOLOv7 model:**
    - Use the prepared dataset to train the model.
    - Ensure the trained model weights are saved and accessible to the application.

