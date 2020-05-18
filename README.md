# COVID19_assignment
Detecting Pneumonia, Non-pneumonia and COVID based on CXR using ResNet18 as an assignment

This is an open ended project to provide DL based solutions.

Task: Develop a DL based model to solve the COVID19Action-Radiology-CXR https://ieee-dataport.org/open-access/covid19action-radiology-cxr 

Submit: Notebook with executed solution on Pytorch, clearly indicating through comments and explained text/header in the .ipynb, detailing

1. How you have split the dataset into train, text, validation?

Approximately 15% data was reserved for testing and rest was used for training and validation. SGD was used to better train the model.

2. Have you taken any methods to compensate for class imbalance?

Image data augmentation like inverting color of images, using only single channel, gaussian noise addition was used to compensate the mnority class and bridge any gap in the number of image data.

3. Any conditions of hot restart during training?

Hot restart was not used in training. However, pre-trained model was downloaded to be used to avoid overfitting and compensate for scarce data.

4. Present the training/validation loss curves and indicate how you have chosen the stopping criteria?

The curves can be seen as plotted above. The stopping criteria was decided when the change in accuracy was < 5%

All the functions/classes used are defined in the same notebook and the corresponding execution has been shown.


Learn about the project which made this dataset: https://covid19action-radiology.github.io/index.html

Understand the need for DL models on Radiology for COVID19 Evidence Based Medicine (particularly CXR in Indian context, with challenges on CT): https://youtu.be/l6z5Qo5sVEI 
