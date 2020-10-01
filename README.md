##Yolov4 model converted to tflite##

Steps for running:
1) Install requirements by running...
	pip install -r requirements.txt

2) Run the following python script to demo detection on images in the folder .data/images
	python detect_jr.py --weights ./checkpoints/yolov4-416.tflite --size 416 --model yolov4 --image ./data/images --framework tflite