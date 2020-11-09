# Skin_Cancer_Image_Classification
To design automated diagnostics of dermatoscopic images of pigmented skin lesions into various cancer and non-cancerous categories.

**Data Source**

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

**Data Description**

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
*dx_type:- Diagnostics type. These are of 4 types namely hist, follow_up, consensus and
confocal.
*age: - The age of the patients. These range from 0 to 85 years of age.
*sex: - The sex orientation of the patient as male, female or unknowns.
*localization: - The certain part of the body where the lesion is limited to. These are of 15
types namely abdomen, acral, back, chest, ear, face, foot, genital, hand, lower extremity,
neck, scalp, trunk, upper extremity and unknowns.



