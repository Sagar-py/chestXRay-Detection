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

---

This project was the final project for the Graduate Course **Deep Learning** at New York University Tandon School of Engineering for the Spring 2021 semester. The course was instructed by [Dr. Chinmay Hegde](https://chinmayhegde.github.io/)
