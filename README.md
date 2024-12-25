# Melanoma Detection Assignment
> A multiclass classification model using a custom convolutional neural network in TensorFlow which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- To build a CNN based model which can accurately detect melanoma.
- Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Create a code to visualize one instance of all the nine classes present in the dataset.
- Chose an appropriate data augmentation strategy to resolve underfitting/overfitting
- Handling class imbalances
- Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
- Choose an appropriate optimiser and loss function for model training 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
### Initial Model:
1.   The model accuracy is very good on train data. But, it's validation accuracy is not good and not comparable to training accuracy.
2.   Also, the training loss is consistently decreasing where as the validation loss is not.
3. This clearly indicates that the current model is **Overfitting**.
### Model with Augmentation:
1. After augmentation the training and validation accuracy are close to each other and it is consistently increased.
2. Same behaviour is observed in training and validation loss and it is consistently decreased.
3. Based on the above two observations it is evident that data augmentation has **Fixed** the **Overfitting** issue.
### Model after handling class imbalance:
1. The Overfitting problem was already addressed with data augmentation and same has been retained even after balancing classes.
2. But, the validation loss is not consistently decreasing which was not the case bfore balancing classes.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow
- matplotlib
- pathlib

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by live session on CNN by IIITB
- RUpGrad course on ML & AI
- 

## Contact
Created by [@chandrakommuri] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
