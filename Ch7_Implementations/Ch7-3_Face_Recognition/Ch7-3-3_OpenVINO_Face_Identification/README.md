#  第七章 邊緣智慧案例實作

## 7.3 人臉辨識

### 7.3.3 OpenVINO身份辨識

由於原OpenVINO中/opt/intel/openvino_2021/deployment_tools/inference_engine/demos/face_recognition_demo/python/face_recognition_demo.py 有使用到OpenCV的 cv2.imshow()，導致程式無法順利執行，所以新增  
from google.colab.patches import cv2_imshow # 新增導入顯示OpenCV格式影像套件包取代cv2.imshow()  
及將其改成Colab的cv2_imshow()  
#cv2.imshow('Face recognition demo', frame)  
cv2_imshow(frame) # 顯示輸入影像，在Colab中用以取代前一行cv2.imshow  

