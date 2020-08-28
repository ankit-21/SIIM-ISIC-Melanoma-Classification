## SIIM-ISIC-Melanoma-Classification
# Kaggle Computer Vision Competition
Melanoma is a deadly disease, but if caught early, most melanomas can be cured with minor surgery. Image analysis tools that automate the diagnosis of melanoma will improve dermatologists' diagnostic accuracy. Better detection of melanoma has the opportunity to positively impact millions of people. We'll dentify Melanoma in images of skin lesions. In particular, we’ll use images within the same patient and determine which are likely to represent a melanoma. Using patient-level contextual information may help the development of image analysis tools, which could better support clinical dermatologists.

# Data
The images are provided in DICOM format. This can be accessed using commonly-available libraries like pydicom, and contains both image and metadata. It is a commonly used medical imaging data format.

Images are also provided in JPEG and TFRecord format (in the jpeg and tfrecords directories, respectively). Images in TFRecord format have been resized to a uniform 1024x1024.

Metadata is also provided outside of the DICOM format, in CSV files.

# CSV Files
train.csv - the training set

test.csv - the test set

sample_submission.csv - a sample submission file in the correct format

# Columns
image_name - unique identifier, points to filename of related DICOM image

patient_id - unique patient identifier

sex - the sex of the patient (when unknown, will be blank)

age_approx - approximate patient age at time of imaging

anatom_site_general_challenge - location of imaged site

diagnosis - detailed diagnosis information (train only)

benign_malignant - indicator of malignancy of imaged lesion

target - binarized version of the target variable
