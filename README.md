# TF2-Object-Detection-Image-Video-Webcam

#  TF2 Object Detection (Images, Video, Webcam)

This project performs **object detection using TensorFlow 2** with a pre-trained SSD MobileNet model. It can detect objects from:

- 📷 Static Images  
- 🎞️ Video Files  
- 🎥 Live Webcam

---

## 🛠️ Technologies Used

- Python 3.x
- TensorFlow 2.x
- OpenCV
- SSD MobileNet V2 (COCO Dataset)

---

## 📁 Project Structure
TF2-Object-Detection-Image-Video-Webcam/
├── detect_from_image.py # Run detection on image
├── detect_from_video.py # Run detection on video
├── detect_from_webcam.py # Run detection from webcam
├── images/ # Folder for input images
├── videos/ # Folder for input videos
├── output/ # Folder to save output files
├── saved_model/ # Pre-trained model files
├── data/mscoco_label_map.pbtxt # Label map
├── requirements.txt # Python dependencies
└── README.md # This file


---

##  How to Use

### 🔹 1. Install dependencies

```bash
pip install -r requirements.txt

🔹 2. Download the pre-trained model
wget http://download.tensorflow.org/models/object_detection/tf2/20200711/ssd_mobilenet_v2_320x320_coco17_tpu-8.tar.gz
tar -xvf ssd_mobilenet_v2_320x320_coco17_tpu-8.tar.gz
mv ssd_mobilenet_v2_320x320_coco17_tpu-8/saved_model ./saved_model


🔹 3. Run detection
📷 Detect from Image:
python detect_from_image.py --image images/test.jpg

🎞️ Detect from Video:
python detect_from_video.py --video videos/sample.mp4

🎥 Detect from Webcam:
python detect_from_webcam.py


Sample Output
Input Image	                                              Detection Output
![detection_output0](https://github.com/user-attachments/assets/dcf84adf-2060-4a98-b015-50ac9d273d28)


![Uploading detection_output0.png…]()
