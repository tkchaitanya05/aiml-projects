# Artificial Intelligence & Machine Learning Projects Portfolio
Repository to share projects I have worked on in data sciences space. These are academic and research projects done during my post graduate program and some of them are the basis of published papers in international journals. Some projects are more for fun and exploring the possibilities with data sciences.

## Football highlights
The aim of this fun project was to detect key Soccer match events to create highlights using Computer Vision (Faster RCNN architecture). This was infact my final capstone project to complete my post graduate study in AIML. As the end product we were able to reduce a 23 min video of football match to generate 4:50 mins of highlights successfully capturing almost all important events in the match.

### Details of Project Files
The project folder contains separate Train and Test python notebooks for the 2 different models used to evaluate the end result. We used Faster RCNN with VGG16 as based model as one approach and Faster RCNN with ResNet50 as another approach. The code for the Keras version of Faster RCNN we referred to was picked from RockyXu66 (resource link: [GitHub](https://github.com/RockyXu66/Faster_RCNN_for_Open_Images_Dataset_Keras)). 

Our best performing model was trained using the file [FasterRCNN_VGG16_Train.ipynb](FasterRCNN_VGG16_Train.ipynb). 254 images annoatated for specific events - **foul, corner kick, penalty kick and goal**, using image labelling tool labelImg and [RoboFlow](https://app.roboflow.com/) were used for training which are shared in [images](images) folder. The file [generate_dataset.py](generate_dataset.py) was used to convert the images and annotations into required data format to be used in the model builing.

### Output of the Model
The output of the Test file [FasterRCNN_VGG16_Test.ipynb](FasterRCNN_VGG16_Test.ipynb) generated a processed highlights video of 4:50 mins. The video was too large to be uploaded here. The image frames identified in the output file [videoplayback_metafile.txt](videoplayback_metafile.txt) under [Test_output_files_VGG16](Test_output_files_VGG16) folder were combined using openCV to generate the output highlights video. 

Below are a few snippets of the model ouput identifying some key moments in the football match video we used for Test:

<picture>
<img alt="Output Goal Image 1" src="/Football_Highlights/Test_output_files_VGG16/Model_Output_test_Goal1.png">
</picture>

<picture>
<img alt="Output Goal Image 2" src="/Football_Highlights/Test_output_files_VGG16/Model_Output_test_Goal2.png">
</picture>

<picture>
<img alt="Output Penalty Kick Image 1" src="/Football_Highlights/Test_output_files_VGG16/Model_Output_test_PenaltyKick1.png">
</picture>

<picture>
<img alt="Output Penalty Kick Image 2" src="/Football_Highlights/Test_output_files_VGG16/Model_Output_test_PenaltyKick2.png">
</picture>

<picture>
<img alt="Output Corner Kick Image2" src="/Football_Highlights/Test_output_files_VGG16/Model_Output_test_CornerKick.png">
</picture>

**Contributors to the project** - Other team members who contributed to the project are: Prashant Kumar, Abhaya Thakur, Nikhil Malhotra, Vigneswaran Sundaramurthy, Shivam Chauhan, 


## Clustering Countries by Covid-19 handling
<!-- Clustering Countries by Covid-19 handling -->
