### Object-Detection
It is a technique of computer vision and image processing that deals with detecting instances of semantic objects of a certain class such as humans, buildings and cars in digital images and videos.
### Requirements
* Keras 2.x
* Python 3.x
* Tensorflow 1.x
### Folder Structure
├── __Code__     
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── fasterRcnnTesting.ipynb  
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── fasterRcnnTraining.ipynb    
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── retinaNet.ipynb    
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── yolo.ipynb    
├── __Architecture__    
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── faster.png  
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── retina.png   
│ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── yolov3.png   
### Dataset 
Satellite Imagery Multi-vehicles Dataset (SIMD). It comprises 5,000 images of resolution 1024 x 768 and collectively contains 45,303 objects in 15 different classes of vehicles including cars,
trucks, buses, long vehicles, various types of aircrafts and boats. The source images are taken from public satellite imagery available in Google Earth and contain images of multiple locations from seven countries.
### 1. Faster RCNN
![Faster RCNN](Architecture/faster.png)
### Quantitative Results
car AP: 0.347720230630157  
trainer AP: 0.11860645967788826  
van AP: 0.6609418589984271  
bus AP: 1.0  
airliner AP: 0.4469653226813752  
truck AP: 0.9783422855171734  
longvehicle AP: 0.9024390243902439  
stairtruck AP: 1.0  
boat AP: 1.0  
other AP: 1.0  
chartered AP: 0.3837540122497782  
propeller AP: 0.8928571428571429  
helicopter AP: 1.0  
pushback AP: 1.0  
fighter AP: 1.0  
mAP = 0.7821084224668123  
### Prediction  
![faster](Result/faster.png)  
### 2. RetinaNet RCNN
![RetinaNet](Architecture/retina.png)
### Quantitative Results
3678 instances of class car with average precision: 0.6550  
446 instances of class truck with average precision: 0.0403  
874 instances of class van with average precision: 0.1199  
222 instances of class longvehicle with average precision: 0.0178  
366 instances of class bus with average precision: 0.0261  
161 instances of class airliner with average precision: 0.5558  
25 instances of class propeller with average precision: 0.0286  
49 instances of class trainer with average precision: 0.0282  
103 instances of class chartered with average precision: 0.1893  
8 instances of class fighter with average precision: 0.0000  
85 instances of class other with average precision: 0.0033  
83 instances of class stairtruck with average precision: 0.0000  
55 instances of class pushback with average precision: 0.0000  
9 instances of class helicopter with average precision: 0.0000  
1820 instances of class boat with average precision: 0.4067  
Inference time for 747 images: 0.3206  
mAP using the weighted average of precisions among classes: 0.4255  
mAP: 0.1381  
### Prediction  
![retina](Result/retina.png)  
### 3. YOLOV3
![YOLOV3](Architecture/yolov3.png)
### Quantitative Results
airliner: 0.4249  
boat: 0.4690  
bus: 0.1306  
car: 0.5915  
chartered: 0.5114  
fighter: 0.0000  
helicopter: 0.0006  
longvehicle: 0.1432  
other: 0.0002  
propeller: 0.1607  
pushbacktruck: 0.0149  
stairtruck: 0.0005  
trainer: 0.2326  
truck: 0.2090  
van: 0.1532  
mAP: 0.2028  
### Prediction  
![yolo](Result/yolo.jpg)  
