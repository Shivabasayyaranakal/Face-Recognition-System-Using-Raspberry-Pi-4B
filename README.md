🚀 Face Recognition System using Raspberry Pi 4B
A face recognition system using Raspberry Pi 4B, OpenCV, and a camera module to detect and recognize faces in real time.
📝 1. Installation & Setup
⚙️ Prerequisites
Raspberry Pi 4B
Raspberry Pi Camera Module or USB Webcam
MicroSD card with Raspberry Pi OS
Internet connection

🔧 Install Dependencies
sudo apt update && sudo apt upgrade -y
sudo apt install python3 python3-pip -y
pip3 install -r requirements.txt

🛠️ Install OpenCV & dlib
pip3 install opencv-python opencv-contrib-python dlib face_recognition numpy

🎥 2. Dataset Collection
Capture images to train the model.
python3 dataset_capture.py
This script will:
Detect faces using OpenCV.
Save images in dataset/person_name/.

🧠 3. Train Face Recognition Model
python3 train_model.py
This will:
Extract face features.
Train and save a model (models/face_trained.yml).

🤖 4. Face Recognition
python3 recognize_faces.py
This script:
Loads the trained model.
Detects and recognizes faces in real time.
