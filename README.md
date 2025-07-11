﻿

﻿# TF2-Object-Detection-Image-Video-Webcam



\#  TF2 Object Detection (Images, Video, Webcam)



This project performs \*\*object detection using TensorFlow 2\*\* with a pre-trained SSD MobileNet model. It can detect objects from:



\- 📷 Static Images  

\- 🎞️ Video Files  

\- 🎥 Live Webcam



---



\## 🛠️ Technologies Used



\- Python 3.x

\- TensorFlow 2.x

\- OpenCV

\- SSD MobileNet V2







---



\## 📁 Project Structure

TF2-Object-Detection-Image-Video-Webcam/

├── detect\_from\_image.py # Run detection on image

├── detect\_from\_video.py # Run detection on video

├── detect\_from\_webcam.py # Run detection from webcam

├── images/ # Folder for input images

├── videos/ # Folder for input videos

├── output/ # Folder to save output files

├── saved\_model/ # Pre-trained model files

├── data/mscoco\_label\_map.pbtxt # Label map

├── requirements.txt # Python dependencies

└── README.md # This file





---







\##  How to Use



\### 🔹 1. Install dependencies



```bash

pip install -r requirements.txt



🔹 2. Download the pre-trained model

wget http://download.tensorflow.org/models/object\_detection/tf2/20200711/ssd\_mobilenet\_v2\_320x320\_coco17\_tpu-8.tar.gz

tar -xvf ssd\_mobilenet\_v2\_320x320\_coco17\_tpu-8.tar.gz

mv ssd\_mobilenet\_v2\_320x320\_coco17\_tpu-8/saved\_model ./saved\_model





🔹 3. Run detection

📷 Detect from Image:

python detect\_from\_image.py --image images/test.jpg



🎞️ Detect from Video:

python detect\_from\_video.py --video videos/sample.mp4



🎥 Detect from Webcam:

python detect\_from\_webcam.py












