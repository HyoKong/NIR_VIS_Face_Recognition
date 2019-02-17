# NIR_VIS_Face_Recognition
NIR-VIS face recognition for CASIA NIR-VIS2.0 dataset, implemented by Pytorch.      
Scripts only for testing and reporting performance.    
With pretrained LightCNN29V2 and proper preprocessing, Rank1 accuracy can achieve 96.7%     

## description
1) extract_features.py      
Apply pretrained deep learning model(LightCNN 9/29) to extract face embedding(128D).            
Compute Rank1 accuracy and accuracy of AR@FAR=0.01.     
It implements the view2 protocal defined by CASIA2.0 dataset.       
2) light_cnn.py
The standard LightCNN model.     
Acess here for more about LightCNN: https://github.com/AlfredXiangWu/LightCNN    

## prerequisite
1) You need to do face detection and face alignment, then crop face images to 112*112.   
You can follow MTCNN to do face detection, but some NIR faces will not be detected.    
A better way is to use SSH face detector, which is introduced in this paper: https://arxiv.org/abs/1708.03979     
2) Download pretrained LightCNN weight.   

