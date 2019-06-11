# Kaggle & Fun
This is the wiki of the __Kaggle&Fun__ project, a project personally driven at my company in order to make profit my colleagues and friends and the _power and fun_ one can have while solving deep learning challenges. The basic approach is to provide a basic foundation of what deep learning is in order to be able to move as quick as possible into the practice of kaggle challenges, as practice makes mastery. 

This git is used in order to agglutinate all material presented in class, tasks to realize as well as organize the code to be available to participants.

## Current challenge:
Kaggle __Histopathologic Cancer Detection__ [challenge](https://www.kaggle.com/c/histopathologic-cancer-detection)

In this competition, you must create an algorithm to identify metastatic cancer in small image patches taken from larger digital pathology scans.

*[PCam] packs the clinically-relevant task of metastasis detection into a straight-forward binary image classification task, akin to CIFAR-10 and MNIST. Models can easily be trained on a single GPU in a couple hours, and achieve competitive scores in the Camelyon16 tasks of tumor detection and whole-slide image diagnosis. Furthermore, the balance between task-difficulty and tractability makes it a prime suspect for fundamental machine learning research on topics as active learning, model uncertainty, and explainability.*

[image]: images/histopathologic.png
![histopatologic][image]

### Data Description
In this dataset, you are provided with a large number of small pathology images to classify. Files are named with an image `id`. The `train_labels.csv` file provides the ground truth for the images in the `train` folder. You are predicting the labels for the images in the `test` folder. A positive label indicates that the center 32x32px region of a patch contains at least one pixel of tumor tissue. Tumor tissue in the outer region of the patch does not influence the label. This outer region is provided to enable fully-convolutional models that do not use zero-padding, to ensure consistent behavior when applied to a whole-slide image.

The original PCam dataset contains duplicate images due to its probabilistic sampling, however, the version presented on Kaggle does not contain duplicates. We have otherwise maintained the same data and splits as the PCam benchmark. 
