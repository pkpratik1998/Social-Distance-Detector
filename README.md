# Social-Distance-Detector

<b>Due to file limit I was unable to push a file in this repository.
So I uploaded the project files on drive. use the link below to download.</b>

<b>link</b>- https://drive.google.com/file/d/17_5mhh6pKa-bkb9hoJWFweca-AsiSptQ/view?usp=sharing


It's a COVID-19 social distance violation detector using OpenCV, Deep Learning, and Computer Vision.

<h3>Project Structure :</h3>
1) The configuration file used to keep the implementation neat and tidy. <br>
2)<i> 'detect_people' </i>utility function, which detects people in video streams using the<b> YOLO object detector.</b> <br>
3) Python driver script, which glues all the pieces together into a full-fledged OpenCV social distancing detector.<br>


<b>The steps to build a social distancing detector include:<b>
1) Apply object detection to detect all people in a video stream.<br>
2) Compute the pairwise distances between all detected people.<br>
3) Based on these distances, check to see if any two people are less than N pixels apart.
