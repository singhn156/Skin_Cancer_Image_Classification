# Skin_Cancer_Image_Classification
To design automated diagnostics of dermatoscopic images of pigmented skin lesions into various cancer and non-cancerous categories.

## Data Source

The International Skin Imaging Collaboration (ISIC) is an international effort to improve
melanoma diagnosis, sponsored by the International Society for Digital Imaging of the Skin
(ISDIS). The ISIC hosted a challenge in 2018 at the Medical Image Computing and Computer
Assisted Intervention (MICCAI) conference in Granada, Spain. Skin cancer is one of the most
common forms of cancer, as reported by the American Cancer Society. While skin cancer is
amenable to early detection by direct inspection, visual similarity with benign lesions makes the
task difficult.
The goal of the challenge was to develop methods for segmentation, clinical attribute detection,
and disease classification in dermatoscopic images.
https://challenge2018.isic-archive.com/

The data set is now available on “Harvard Dataverse” which is a free data repository open to all
researchers from any discipline, both inside and outside of the Harvard community, where you can
share, archive, cite, access, and explore research data.
https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T

Alternatively the data is also available on Kaggle. Kaggle is a subsidiary of Google LLC and is an
online community of data scientists and machine learning practitioners. It allows users to find and 
publish data sets, explore and build models in a web-based data-science environment, work with
other data scientists and machine learning engineers, and enter competitions to solve data science
challenges.
https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000

## Data Description

HAM10000 ("Human Against Machine with 10000 training images") dataset is a large collection
of multi-source dermatoscopic images of common pigmented skin lesions from different
populations, acquired and stored by different modalities. The dataset includes lesions with multiple
images, which can be tracked by the lesion_id-column within the HAM10000_metadata file. The
final dataset consists of 10015 dermatoscopic images and serve as a training set for academic
machine learning purposes. It consists of 7 columns and 10015 rows.
The columns are as listed below exactly how they are present in the dataset:

* lesion_id: - The unique id of a skin lesion for a patient.
* image_id: - Contains unique values referring to each of the image present in the image file.
* dx: - A representative collection of all diagnostics category in the realm of pigmented skin
lesions. These are of 7 types namely Akiec, bcc, bkl, df, mel, nv and vasc.
* dx_type:- Diagnostics type. These are of 4 types namely hist, follow_up, consensus and
confocal.
* age: - The age of the patients. These range from 0 to 85 years of age.
* sex: - The sex orientation of the patient as male, female or unknowns.
* localization: - The certain part of the body where the lesion is limited to. These are of 15
types namely abdomen, acral, back, chest, ear, face, foot, genital, hand, lower extremity,
neck, scalp, trunk, upper extremity and unknowns.

## Methology

* K-Nearest Neighbour 
* Support Vector Machine
* Artificial Neural Network
* Convolutional Neural Network
* Transfer Learning Mobilnet

## Results and Comparison

* TABLE: Comparison of Classifiers

CLASSIFIER               |                           ACCURACY                  |        TRAINING TIME
-------------------------|-----------------------------------------------------|------------------------------

K-Nearest Neighbour(KNN) |        Manhattan Distance 67.3%  Euclidean Distance 68.42%   |              40 minutes
-------------------------|------------------------------------------------------------|------------------------------

Support Vector Machine (SVM) | Polynomial Kernel 73.18%  Radial Basis Function Kernel 72.51%  |          30 minutes
-----------------------------|-----------------------------------------------------------------|-----------------------

Artificial Neural Network (ANN) | Single Hidden Layer 72.3%  Hidden Layer 71.7%  Hidden Layer 71.48% | 20 minutes (using 12 GB NVIDIA Tesla K80 GPU)
--------------------------------|---------------------------------------------------------------------|----------------------------------------------

Convolutional Neural Network (CNN) | Without Data Augmentation (10015 Images) 75.5%   |       2 hours 15 minutes (using 12 GB NVIDIA Tesla K80 GPU)
------------------------------------|--------------------------------------------------|-------------------------------------------------------------

Convolutional Neural Network (CNN) (MobileNet Architecture)| With Data Augmentation (34588 Images) 86.14% | 3 hours 35 minutes (using 12 GB NVIDIA Tesla K80 GPU)
-----------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------


* Plot and Selected Model Evaluation 

![Plot Skin](https://user-images.githubusercontent.com/38158849/98530470-f6786b80-22a4-11eb-9dc4-20b4d677e38c.png)

![Validation](https://user-images.githubusercontent.com/38158849/98531220-0c3a6080-22a6-11eb-88da-bf1baeb453b4.png)

![Testing](https://user-images.githubusercontent.com/38158849/98531251-16f4f580-22a6-11eb-86fc-ef000b1b6a93.png)

* Output Or Prediction of Newly Skin Images

![Prediction1](https://user-images.githubusercontent.com/38158849/98531760-d2b62500-22a6-11eb-8fde-f0133afb5e67.png)

![Prediction2](https://user-images.githubusercontent.com/38158849/98531768-d649ac00-22a6-11eb-8b5b-2638985737c8.png)


Follow me on [Linkedin](https://www.linkedin.com/in/nikhil-singh-9a5324b4/)
