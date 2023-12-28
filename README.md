# Detectron2-Mask-Detection
Problem Statement : Creating a Detectron2 custome object detection model to detect Mask.

Dataset link : https://www.kaggle.com/datasets/aditya276/face-mask-dataset-yolo-format


# Mask detection on detectron2 colab file

The detectron model used for creating this model is 'faster_rcnn_R_50_C4', a prebuild model present in detectron2 model_zoo module.

The input data is first annotated using LabelMe annotation tool, there are 2 classes made on the training and testing images named 'Mask' and 'No Mask'. After annotating the images the json format is converted into desired COCO format required by detectron2.

There 1035 training dataset instances in which 885 instances are of 'Mask' and 150 are of 'No Mask' and for testing there are 60 total instances out of which 32 are of 'Mask' and 28 of 'No Mask'.

The model is trained on CUDA processor on 128 images per batch for 500 iterations

# Results of model
The images below are the models prediction to detect the two classes 'Mask' and 'No Mask'

# Original image
![predicted image1](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/df15b241-0c58-46ce-b6fe-7c2a4ccd277d)

# Predicted annoatations 
![annotated image 1](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/103c25c6-5d40-4888-baab-92f8147066c2)

# Original image
![predicted image2](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/775cac8a-b4e5-4006-9f03-dcd7dc598583)

# Predicted annoatations 
![annotated image 2](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/3cbcfb1e-7dbd-4dbb-a347-ed57c7a5dce4)

# Model Evaluation 

On training images the model is able to get around 45% AP (Average Precision)
![training](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/ebdc53e0-68ed-4972-a4d0-a7b2d58b9dd0)


On testing images the model is able to get around 21% AP (Average Precision)
![testing](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/03175941-1640-4b8d-bbf9-42efcc552bb6)

# Flask Output
![flask image1](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/6bdc050c-880a-47d6-b0d5-0442bcdd4489)
![flask image2](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/a741d613-ee64-4cf0-a9c8-f471afaba550)
![flask image 3](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/2d7abec0-c49e-401a-bb7a-d8f8c56fe631)
![flask image4](https://github.com/nehach29/Flask-API-and-Streamlit-of-Detectron2-model/assets/109617232/769104f9-7ec0-4d56-be6c-d3b354ee3235)





