Project Overview: Object Detection and Tracking


**Libraries Used:

*FFmpeg:				A multimedia framework for processing video and audio. Used to handle video input/output.

*os: 				For file path manipulations and interacting with the operating system.

*cv2 (OpenCV): 		A library for computer vision tasks, including image and video processing.

*matplotlib.pyplot: 	For visualizing images and results in a notebook environment.

*numpy: 				For numerical operations on arrays, particularly useful for image data.

*IPython.display: 	To embed videos and display HTML content within Jupyter notebooks.


**Data Used:

*City Traffic.mp4:			 				The video dataset containing scenes of traffic, which will --be analyzed for vehicle and person detection.

*coco_class_labels.txt:		 				A file containing the class labels for the objects (e.g., vehicles, -persons) that the model can detect.

*frozen_inference_graph.pb:	 				The serialized TensorFlow model containing the trained weights and --architecture for object detection.

*ssd_mobilenet_v2_coco_2018_03_29.pbtxt: 	A text file that provides a human-readable description of the TensorFlow model's -architecture.



**Workflow Overview:

*Setup Environment:
	-Install necessary libraries (FFmpeg, OpenCV, etc.).
	-Load the model and labels.

*Process Video:
	-Open the video file using OpenCV.
	-Read frames from the video.

*Object Detection:
	-For each frame, perform the following:
		-Convert the frame to the format required by the model.
		-Run inference to detect objects.
		-Draw bounding boxes around detected vehicles and persons.

*Display Results:
	-Use Matplotlib to visualize the detected objects in frames.


Open the Main.ipynb file in collab and run it
