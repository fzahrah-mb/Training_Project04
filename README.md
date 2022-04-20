# Modified U- Net Convolutional Neural Network for Cell Neuclei Detection
_Using a Modified U- Net Convolutional Neural Network for Cell Neuclei Detection using Semantic Segmentation_

## Description

- The model utilises the [2018 Data Science Bowl Dataset from Kaggle][df1] to detect the cell nuclei using Semantic Segmentation.
- In a summary, the dataset contains a large number of segmented nuclei images. The images were acquired under a variety of conditions and vary in the cell type, magnification, and imaging modality.
- A Modified U- Net Convolutional Neural Network is used for the project because of the relatively high number of the images and masks for Semantic Segmentation.

## Methodology
#### The project can be divided into several sections:
- Data Loading
    - All of the data, images and masks are loaded into each respective array.
- Data preprocessing
    - The data are normalized.
    - The data are categorised into train, validation, and test set.
- Model Definition
    - The project has applied Transfer Learning from MobileNetV2 as the base model. MobileNetV2 is chose because it is a relatively lightweight model but still delivers an acceptable model accuracy.
- Model Modification
    - Some modifications are made at the end of the base model to complete it:
        - Addition of 1 dense output layer.
- Model Training
- Model Evaluation

## Results
- The training was set to run for 20 epochs only due to the huge amount of time take to complete an epoch.
- Model evaluation was done after model training and the results are:
    - Test loss = 0.35
    - Test accuracy = 0.86

## License
Copyright (c) [2022] [Fatimah Zahrah binti Mohd Badry]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [df1]: <https://www.kaggle.com/competitions/data-science-bowl-2018/overview>