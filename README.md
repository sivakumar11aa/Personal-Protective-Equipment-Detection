🦺 Construction Site Safety Detection using YOLOv8
📌 Overview

This project implements a real-time Personal Protective Equipment (PPE) detection system for construction sites using YOLOv8. The system detects whether workers are complying with safety regulations such as wearing hard hats, masks, and safety vests through live webcam feed or video input.

The goal of this project is to enhance workplace safety monitoring by automatically identifying safety violations and compliant behavior in real time.

🚀 Features

🔍 Real-time object detection using YOLOv8

🎥 Supports webcam and video file input

🦺 Detects multiple safety-related classes:

Hardhat / No-Hardhat

Mask / No-Mask

Safety Vest / No-Safety Vest

Person, Machinery, Vehicle, Safety Cone

🎨 Color-coded bounding boxes:

🔴 Red → Safety violation

🟢 Green → Safety compliant

🔵 Blue → Other objects

⚡ Optimized for real-time performance

🧠 Tech Stack

Python

YOLOv8 (Ultralytics)

OpenCV

cvzone

PyTorch

📂 Dataset

The dataset used for training was obtained from Roboflow Universe:

🔗 Construction Site Safety Dataset (YOLOv8 format)
https://universe.roboflow.com/roboflow-universe-projects/construction-site-safety/dataset/28/download/yolov8

Dataset Highlights:

Annotated images for PPE and construction-site objects

Multiple safety violation and compliance classes

Preprocessed and compatible with YOLOv8 training pipeline

📁 Project Structure
├── PPEDetection.py        # Real-time detection script
├── ppe.pt                # Trained YOLOv8 model weights
├── requirements.txt      # Project dependencies
├── README.md             # Project documentation

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/construction-site-safety-detection.git
cd construction-site-safety-detection

2️⃣ Create Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

3️⃣ Install Dependencies
pip install -r requirements.txt

▶️ Running the Project
✅ Run with Webcam
python PPEDetection.py


Ensure your webcam is accessible.
Press Q to exit the application.

✅ Run with Video File

Uncomment and modify the following line in PPEDetection.py:

cap = cv2.VideoCapture("path_to_video.mp4")

🧪 How It Works

Captures frames from webcam/video using OpenCV

Passes each frame to YOLOv8 for inference

Extracts bounding boxes, class labels, and confidence scores

Applies safety rules and assigns colors

Displays annotated frames in real time

📊 Use Cases

Construction site safety monitoring

Industrial workplace compliance checks

Smart surveillance systems

AI-based occupational safety solutions

🔮 Future Improvements

🚨 Real-time alert system for violations

📈 Safety compliance analytics dashboard

📱 Web / Mobile deployment (Streamlit / Flask)

🎯 Model optimization for edge devices

📹 Multi-camera support

👨‍💻 Author

Siva Kumar
Machine Learning & AI Enthusiast
Focused on Computer Vision & Real-Time AI Systems

📜 License

This project is for educational and research purposes.
Dataset credit belongs to Roboflow Universe.
