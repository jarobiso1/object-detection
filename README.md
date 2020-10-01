Below Are instructions for running a Yolov4 model converted to tflite to detect handguns in an image

Steps for running:
1) Install requirements by running...
	pip install -r requirements.txt
	
2) Downloading the yolov4 model from https://ibm.ent.box.com/folder/122722273224?s=2dcij8tsllc43em0ukf37ykkfpw6ilym and adding it to the checkpoints folder

3) Run the following python script to demo detection on images in the folder .data/images
	python detect_jr.py --weights ./checkpoints/yolov4-416.tflite --size 416 --model yolov4 --image ./data/images --framework tflite
	
The Google Colab notebook I used to create and train the model is tensorflow-yolov4.ipynb

Other resources I used to create the YoloV4 object dection model and to convert it to TFLite and TRT are located below:

Handgun Dataset: (Links under 3.)
https://sci2s.ugr.es/weapons-detection

Convert to TFLite:
https://github.com/hunglc007/tensorflow-yolov4-tflite

YOLOv4 Implementation:
https://github.com/AlexeyAB/darknet


