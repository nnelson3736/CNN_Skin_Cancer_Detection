# CNN_Skin_Cancer_Detection
CNN model for early detection of Melanoma which is a type of Skin Cancer

We want to build a CNN-based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)



## General Information
- The project is to build a CNN model which can help detect Melanoma. It is a type of cancer and early detection can help save alot of lives.
- In order to build the model we are using a dataset consisting of 2357 images of malignant and bening oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC).
- The Dataset contains the images of the following diseases:
1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion

- With a good CNN model we can detect the Melanoma early in patients and it can help doctors make timely decisions and to start the medications. Which can in turn help the doctors in saving many lives. This model is no way a replacement of the existing medical tests that are available to detect the condition. This is only an added tool which can be used along with the other existing procedures and methods.



## Conclusions
- During our initial stage of Model building we found out that the Base Model that we built was overfitting. It was performing good on the training data but was failing miserably in the Validation data. In the base model we used 3 Convolutional Layers with 3 Pooling Layers.
- To fix the Overfitting we did some data augmentation. We modified the existing images like rotating and flipping them and also introduced a dropout layer. This time the overfitting problem was fixed but the model was not giving good results as the accuracy was down to about 58%. But at least the accuracy and the validation accuracy were in line with each other.
- We checked the data for distribution of the images of different classes or in our case the diseases an dfound out that images of some of diseases were very few as compared to the others and this could be hampering the preformance of the model cause our model does not have enough samples for training on those diseases an dwould have difficulty detecting them. and Hence we used the augmentor and added about 500 images of each classes by using the augmenting methods. This helped us get enough data to train the model.
- Conclusion 4 from the analysis


## Technologies Used
- Numpy
- Pandas
- TensorFlow
- Augmentor


## Contact
Created by [@nnelson3736] - feel free to contact me!
