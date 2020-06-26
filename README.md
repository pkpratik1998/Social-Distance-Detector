# Social-Distance-Detector


It's a COVID-19 social distance violation detector using OpenCV, Deep Learning, and Computer Vision.

<h1>Dependencies:</h1>
1) Python >= 3.6.<br>
2) OpenCV.<br>
3) YOLO V3.<br>
4) NVIDIA GPU.

<h2>Download YOLOv3:</h2> <b>link</b>- https://drive.google.com/drive/folders/1hUBKEFeGoi8KIyIpJHpE2kdBE4x13iYA?usp=sharing

Put the downloaded folder as per below directory structure.

$ tree --dirsfirst
.
├── libraries
│   ├── __init__.py
│   ├── detection.py
│   └── social_distancing_config.py
├── yolo-coco
│   ├── coco.names
│   ├── yolov3.cfg
│   └── yolov3.weights
├── output.avi
├── Subway.mp4
└── social_distance_detector.py
2 directories, 9 files

<h3>Project Structure :</h3>
1) The configuration file used to keep the implementation neat and tidy. <br>
2)<i> 'detect_people' </i>utility function, which detects people in video streams using the<b> YOLO object detector.</b> <br>
3) Python driver script, which glues all the pieces together into a full-fledged OpenCV social distancing detector.<br>


<b>The steps to build a social distancing detector include:<b>
1) Apply object detection to detect all people in a video stream.<br>
2) Compute the pairwise distances between all detected people.<br>
3) Based on these distances, check to see if any two people are less than N pixels apart.
