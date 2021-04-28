# Chest X-ray Abnormalities Detection

When we have a broken arm, radiologists help save the day - and the bone. These doctors diagnose and treat medical conditions using imaging techniques like CT and PET scans, MRIs, and X-rays. Yet, as it happens when working with such a wide variety of medical tools, radiologists face many daily challenges, perhaps the most difficult being the chest radiograph. The interpretation of chest X-rays can lead to a medical misdiagnosis, even for the best practicing doctor. Computer-aided detection and diagnosis systems would help reduce the pressure on doctors at metropolitan hospitals and improve diagnostic quality in rural areas.

Existing methods of interpreting chest X-ray images classify them into a list of findings. There is currently no specification of their locations on the image which sometimes leads to inexplicable results. A solution for localizing findings on chest X-ray images is needed for providing doctors with more meaningful diagnostic assistance.


## Using the detectron2 training approach
Detectron2 is Facebook AI Research's next generation software system that implements state-of-the-art object detection algorithms. It is a ground-up rewrite of the previous version, Detectron, and it originates from maskrcnn-benchmark.

[Link to the Repository](https://github.com/facebookresearch/detectron2)

![](https://user-images.githubusercontent.com/1381301/66535560-d3422200-eace-11e9-9123-5535d469db19.png)

## Table of Contents
- [Dataset Preparation](#Dataset-Preparation)
- Installation
- Exploratory Data Analysis: Distribution between Normal and Abnormal Classes
- Data Visualization and Augmentation
- Defining the CNN Models
- Training utils
- Training Scripts
- Prediction on Validation and Test Dataset

## Dataset Preparation
