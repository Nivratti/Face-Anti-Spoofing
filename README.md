# Face-Anti-Spoofing
A simple face anti-spoofing based on CNN trained with HSV + YCrCb color feature.

![Network Architecture](https://github.com/Oreobird/Face-Anti-Spoofing/raw/master/model.png) 

### Dependencies:<br>
		dlib >= 19.17.0
		tensorflow >= 1.12.0
		keras >= 2.2.4
		numpy >= 1.11.1
		scipy >= 0.14
		opencv-python >= 3.4.3

### Usage:<br>
* Data prepare:<br>
		1) Download train data and model file from:<br>
		https://drive.google.com/drive/folders/1HH7t366ZCdwTUcWpVGSY7kY0yZjoWCcn?usp=sharing
		
		2) untar data and model to your project dir
* Train model:<br>
		python data/NUAA/gen_label.py
		python main.py --train=True
* Test online via camera:<br>
		python main.py --online=True
