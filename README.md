Quick fix by Jordan of [this repository](https://github.com/jhasuman/potholes-detection/), as descrirbed by [an issue opened by Jordan on same repository](https://github.com/jhasuman/potholes-detection/issues/6).

Steps taken to fix issues:

1. Modified [config.json](https://github.com/JordanMicahBennett/potholes-detection/blob/master/config.json), to include "backend":"Full Yolo" in model object. (This was missing from [the original config.json in main repository](https://github.com/jhasuman/potholes-detection/blob/master/config.json), and lead to a run-time error.)

2. To remove **_full_yolo_backend_** error that appeared at run time out of the box, I downloaded [full_yolo_backend.h5 from another repository](https://github.com/rodrigo2019/keras_yolo2/releases/tag/pre-trained-weights) to directory of this downloaded repository.

3. Successfully ran code on [this random pic with potholes that I took from google](https://d1ix0byejyn2u7.cloudfront.net/drive/images/uploads/headers/ws_cropper/1_0x0_1410x520_0x520_potholes.jpg).

Test data from [said random pic with potholes](https://d1ix0byejyn2u7.cloudfront.net/drive/images/uploads/headers/ws_cropper/1_0x0_1410x520_0x520_potholes.jpg):

Input: 
![image](https://user-images.githubusercontent.com/3666405/61832223-0eb94280-ae36-11e9-97f5-c0f52377cfaf.png)

Result:
![image](https://user-images.githubusercontent.com/3666405/61832244-2264a900-ae36-11e9-8b0a-7ef6e2fcf35e.png)
