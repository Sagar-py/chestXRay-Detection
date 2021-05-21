# Chest X-ray Abnormalities Detection

Download the test and training dataset from the given link: [Chest X-ray Resized PNG (256 x 256)](https://www.kaggle.com/xhlulu/vinbigdata-chest-xray-resized-png-256x256?select=test)

---

## Introduction
When we have a broken arm, radiologists help save the day - and the bone. These doctors diagnose and treat medical conditions using imaging techniques like CT and PET scans, MRIs, and X-rays. Yet, as it happens when working with such a wide variety of medical tools, radiologists face many daily challenges, perhaps the most difficult being the chest radiograph. The interpretation of chest X-rays can lead to a medical misdiagnosis, even for the best practicing doctor. Computer-aided detection and diagnosis systems would help reduce the pressure on doctors at metropolitan hospitals and improve diagnostic quality in rural areas.

Existing methods of interpreting chest X-ray images classify them into a list of findings. There is currently no specification of their locations on the image which sometimes leads to inexplicable results. A solution for localizing findings on chest X-ray images is needed for providing doctors with more meaningful diagnostic assistance.

## Goal
The goal is to automatically localize and classify 14 types of thoracic abnormalities from chest radiographs while working with a dataset consisting of 18,000 scans that have been annotated by experienced radiologists. The model can be trained with 15,000 independently-labeled images and will be evaluated on a test set of 3,000 images. 

These annotations were collected via VinBigData's web-based platform, [VinLab](https://vindr.ai/vinlab). Details on building the dataset can be found in the paper [“VinDr-CXR: An open dataset of chest X-rays with radiologist's annotations”](https://arxiv.org/pdf/2012.15029.pdf).

---

## Instructions
1. Download the dataset from the given [link](https://www.kaggle.com/xhlulu/vinbigdata-chest-xray-resized-png-256x256?select=test) and place it in the same folder as that of the repository. The dataset was not added to the repository as it is larger than the maximum storage limit permitted by GitHub.
2. Run the [notebook-train.ipynb](https://github.com/Sagar-py/chestXRay-Detection/blob/main/notebook-train.ipynb) to train. Note that training the model without a cluster could take hours.
3. Run the [notebook-prediction.ipynb](https://github.com/Sagar-py/chestXRay-Detection/blob/main/notebook-prediction.ipynb) for prediction.
4. In the last cell of [notebook-prediction.ipynb](https://github.com/Sagar-py/chestXRay-Detection/blob/main/notebook-prediction.ipynb), rename the file where you would want the predicted values to be stored.

## References
1. [VinLab: Data Platform for Medical AI](https://vindr.ai/vinlab)
2. [VinDr-CXR: An open dataset of chest X-rays with radiologist’s annotations](https://arxiv.org/pdf/2012.15029.pdf)
3. [Detectron2 installation instructions](https://github.com/facebookresearch/detectron2/blob/master/INSTALL.md)
4. [Mask R-CNN](https://arxiv.org/abs/1703.06870)
5. [Detectron2 Beginner Tutorial Collab](https://colab.research.google.com/drive/16jcaJoc6bCFAQ96jDe2HwtXj7BMD_-m5#scrollTo=QHnVupBBn9eR)
6. [Detectron2 DataLoader and comparing Models](https://detectron2.readthedocs.io/en/latest/tutorials/data_loading.html)
7. [Detectron2 Compare Models Augmentation](https://www.kaggle.com/dhiiyaur/detectron-2-compare-models-augmentation/#data)
8. [COCOdataset detection-eval](http://cocodataset.org/#detection-eval)
9. [COCOdataset keypoints-eval](http://cocodataset.org/#keypoints-eval)
10. [Detectron2 JSON Evaluator](https://github.com/facebookresearch/Detectron/blob/a6a835f5b8208c45d0dce217ce9bbda915f44json_dataset_evaluator.py)
11. [Understanding Loss Evaluation Hook and training on Detectron2 with a Validation set](https://ortegatron.medium.com/training-on-detectron2-with-a-validation-set-and-plot-loss-on-it-t6449418fbf4)
12. [Understanding Albumentations](https://github.com/albumentations-team/albumentations)
13. [Visualizing the data on detectron2 and spatial level transformations](https://github.com/facebookresearch/detectron2/blob/22b70a8078eb09da38d0fefa130d0f537562visualize_data.py)
14. [Prediction Batches](https://github.com/sphinx-doc/sphinx/issues/4258)

---

This project was the final project for the Graduate Course **Deep Learning** at New York University Tandon School of Engineering for the Spring 2021 semester. The course was instructed by [Dr. Chinmay Hegde](https://chinmayhegde.github.io/)
