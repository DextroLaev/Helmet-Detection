# Helmet-Detection
# Task for internship
    
   I had used a dataset from kaggle to train the model, I have created a set for train data and a set for test data. The link of the dataset is given below.
   
   In this I had used yolo pre-trained model. For the helmet detection I trained the model on the custom data downloaded from kaggle.
   To count the number of helmets, I just found the total number of bounding boxes in each frame of the video and the total numebr of bounding boxes on the rendered video itself.
   
 ## Steps to run the model on the test videos  
  
   ### 1. Clone the repository on the system:
   
        git clone https://github.com/DextroLaev/Helmet-Detection
        
   This might take sometime as in this repository there is some zip files that are larger in size. Once the repository is cloned, follow the next step.
   
   ### 2. Unzip all the zip files:
      
        unzip model_data.zip
        
        unzip testvideos.zip
        
        unzip dataset.zip
   
   Once the zip files are unzipped, check that your folder structure should match with given folder structure.
   
         Helmet-Detection
            | 
            |-> checkpoints -> contain additonal files inside it.
            |-> model_data -> contain additonal files inside it.
            |-> dataset
                  |
                  |-> test -> contains xml and image files.
                  |-> train -> contains xml and image files.
            |-> tools -> contain additional files inside it.
            |-> yolov3 -> contain additional files inside it.
            |-> deepsort -> contain additional files inside it.
            |-> log -> contain additional files inside it.
            |-> detection_custom.py
            |-> requirements.txt
            |-> detection_demo.py
            |-> train.py
            |-> evaluate_mAP.py
            |-> object_tracker.py
            |-> collect_training_data.py
            |-> also it should have 2 test videos
    
   If the folder structure matches, move to the following step.
    
   ### 3. Install the required libraries:
    
        pip install -r requirements.txt
              
                    or
                    
        pip3 install -r requirements.txt
   
   ### 4. Now its time to detect the helmet on the test videos given.
        
         python detection_custom.py
                  
                    or
        
         python3 detection_custom.py
   
   The above python code might take sometime according to the specifications of the system. After the python code executed successfully, 2 new video files will be created, play the video files.
