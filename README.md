Automatic Car Plate Recognition
===============================

Project Overview
----------------

License plate recognition (LPR) plays a crucial role in traffic management, law enforcement, and security systems. This project focuses on implementing an automatic car plate recognition system using machine learning techniques. The aim is to develop a system capable of accurately identifying and segmenting license plates from images, overcoming challenges such as variations in lighting, weather conditions, and image distortion.

Group Members
-------------

*   Jason Wu
*   Yuan Chen
*   Jui-Wei Chang

Problem Statement
-----------------

The diversity in license plate characters poses a significant challenge in accurate identification and segmentation. Traditional LPR systems follow a multi-step approach, leading to time-consuming processes and errors. To address this, we propose combining YOLOv8 for license plate detection and LPRNet for end-to-end recognition, aiming for accuracy and efficiency.

Background and Pipeline
-----------------------
![alt text](https://github.com/ChenBoYam/EEP567-Final-Project/blob/8584fb17cb8998c17ed8ba91493f114ab947f0c6/pipeline.png?)
We utilize YOLOv8 for license plate detection due to its speed and accuracy. YOLOv8 employs a single deep neural network to identify objects and their bounding boxes. LPRNet, on the other hand, offers an efficient solution for license plate recognition by eliminating the need for pre-segmentation.

Dataset and Preprocessing
-------------------------

We utilize the CCPD2020 dataset, focusing on a subset featuring license plates of green-colored new energy vehicles. The dataset is divided into training, validation, and testing sets, containing images annotated with specific formats for license plate information.

YOLOv8
------

YOLOv8 is trained using the CCPD2020 dataset with hyperparameters optimized for performance. Challenges encountered during training include CUDA version issues and file path discrepancies, which were resolved through troubleshooting.

LPRNet
------

LPRNet is integrated into the workflow for license plate number recognition. Despite challenges in recognizing Chinese characters accurately, LPRNet achieves high accuracy scores with rapid processing speeds.

Experimental Results and Analysis
---------------------------------
![alt text](https://github.com/ChenBoYam/EEP567-Final-Project/blob/d4074602f536ce6060f76020b93a1bc054a92e9f/confusion.png)
After training YOLOv8, we achieved high precision and recall scores. Challenges such as losses being zero and file path issues were addressed through problem-solving. 
![alt text](https://github.com/ChenBoYam/EEP567-Final-Project/blob/d4074602f536ce6060f76020b93a1bc054a92e9f/result.png)
Analysis reveals the importance of robust datasets for training and potential areas for improvement in recognizing Chinese characters accurately.

Future Work
-----------

Future work includes improving multilingual recognition capabilities and promoting the use of car plate numbers tied to driver's credit cards for automated payment processes.

Roles and Responsibilities
--------------------------

*   Data processing: Jason Wu
*   YOLOv8: Jui-Wei Chang
*   LPRNet: Yuan Chen

