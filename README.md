# Artificial Intelligence & Machine Learning Projects Portfolio
Repository to share projects I have worked on in data sciences space. These are academic and research projects done during my post graduate program and some of them are the basis of published papers in international journals. Some projects are more for fun and exploring the possibilities with data sciences.

## Football highlights
The aim of this fun project was to detect key Soccer match events to create highlights using Computer Vision (Faster RCNN architecture). This was infact my final capstone project to complete my post graduate study in AIML. As the end product we were able to reduce a 23 min video of football match to generate 4:50 mins of highlight video successfully capturing almost all important events in the match.

### Details of Project Files
The project folder contains separate Train and Test python notebooks for the 2 different models used to evaluate the end result. We used Faster RCNN with VGG16 as based model in one approach and Faster RCNN with ResNet50 in another approach. The code for the Keras version of Faster RCNN we referred to was picked from RockyXu66 (resource link: [GitHub](https://github.com/RockyXu66/Faster_RCNN_for_Open_Images_Dataset_Keras)). 

Our best performing model was trained using the file [FasterRCNN_VGG16_Train.ipynb](/Football Highlights/FasterRCNN_VGG16_Train.ipynb). Data used for traininig was captured from football images and videos (converted to image frames) obtained from the internet and annoatated for specific events - foul, corner kick, penalty kick and goal, using image labelling tool labelImg and later using [RoboFlow](https://app.roboflow.com/). The 254 images used for training are shared in [images](/Football Highlights/images) folder. The file [generate_dataset.py](/Football Highlights/generate_dataset.py) was used to convert the images and annotations into required data format to be used in the model builing.

### Output of the Model
The output of the Test file [FasterRCNN_VGG16_Test.ipynb](/Football Highlights/FasterRCNN_VGG16_Test.ipynb) generated a processed highlights video of 4:50 mins. The video was too large to be uploaded here. The image frames identified in the [videoplayback_metafile.txt](/Football Highlights/Test output files VGG16/videoplayback_metafile.txt) part of the 'Test Output files VGG16' folder were combined using openCV to generate the output highlights video. 

Below are a few snippets of the model ouput identifying some key moments in the football match video we used for Test:

![Output Goal Image1](/Football Highlights/Test output files VGG16/Model_Output_test_Goal1.png)

![Output Goal Image2](/Football Highlights/Test output files VGG16/Model_Output_test_Goal2.png)

![Output Penalty Kick Image1](/Football Highlights/Test output files VGG16/Model_Output_test_PenaltyKick1.png)

![Output Penalty Kick Image2](/Football Highlights/Test output files VGG16/Model_Output_test_PenaltyKick2.png)

![Output Corner Kick Image2](/Football Highlights/Test output files VGG16/Model_Output_test_CornerKick.png)

### Contributors to the project
Other team members who contributed to the project are: Prashant Kumar, Abhaya Thakur, Nikhil Malhotra, Vigneswaran Sundaramurthy, Shivam Chauhan, 

## Clustering Countries by Covid-19 handling

<!-- Football highlights -->
<!-- Clustering Countries by Covid-19 handling -->
