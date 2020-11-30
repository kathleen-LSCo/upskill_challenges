# No-code Platform Challenge

## Overview

Your goal for this challenge is to train a machine learning model to classify images of Levi's jeans according to fit, and then use that trained model to predict fits for randomized jean images: 

![Image Classification Diagram](https://github.com/fellowship/upskill/blob/master/imgs/cv_model_diagram.png)

The challenge has three main steps:

1. Build a training data set of jean images.
2. Train a Computer Vision model using your data set.
3. Use your trained model to classify images of Levi's jeans according to fit.

Download and use [Lobe.ai](https://lobe.ai/) to complete this challenge. Lobe is a no-code machine learning platform you can use to lable data, train models, and make predictions without any prior code or machine learning knowledge. Refer to the [website](https://lobe.ai/) for more information on how to use the platform.

## Instructions

In the [data repository](https://github.com/fellowship/upskill/tree/master/challenges/Platform/data) you'll find a dataset of 40 randomized jean images. Each of the jeans belongs to one of four fits:

- **Men 501**
- **Men 511**
- **Women 501** 
- **Women 721**

Your goal for this challenge is to train and use a model to predict which fit each randomized image belongs to. The model must predict exactly one of the following labels for each image: 

- **m_501**
- **m_511**
- **w_501**
- **w_721**

Start by building a data set of training images from the web. Your dataset will have to include images from each of the 4 styles, and can't include any of the 40 images from the challenge data. While building your dataset make sure you re-name the images to reflect the fit and image number: m_501_1.jpg, m_501_2.jpg, etc. 

_Hint: the 40 images in the challenge data were scraped from the Levi's website; you may need to look elsewhere for some your data._

Once you have your data organized, named, and numbered you should use Lobe to assign machine learning labels to each image: m_501, w_501, etc. With labeled data in Lobe you can train the model and use it to predict a fit for all the images in the challenge data.

Submit the required deliverables no later than January 28, 2021 [here](link_to_submission_form).

## Guidelines

- None of the randomized images from the challenge data should be in your data (that's data leakage!)
- Your training data should contain fewer images than the challenge data set (<74 images).
- The training data should be as small as possible, i.e. you want to maximize the performance of the model while using the smallest possibel training data set.
- Image labels in Lobe must exactly match one of the following: m_501, m_511, w_501, w_721.
- Don't hand-label the challenge images: you must use a model to predict the fit.
- Make sure you're capable of discussing your methodology and solution during an interview.

## Deliverables

Submit your solution [here](link_to_submission_form) as individual zip files. There are two distinct files you need to submit:

- Your predictions for the jean images: A CSV file containing the image file names and the corresponding predictions. The CSV file should be named _**yourfirstname_yourlastname_predictions.csv**_ and have the following format when viewed in Excel:

| file_name        | prediction |
|------------------|------------|
| 1kDc10mxMfle.jpg | m_501      |
| 5NtNguD8pCKo.jpg | w_721      |

- Your training data: The training data set you used to train your model, including image labels as file names, in a compressed folder named _**yourfirstname_yourlastname_training_data.zip**_