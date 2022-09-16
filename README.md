# EC_601_Project1
## Introduction
Visual Question Answering (VQA) is the system that combines Knowledge Representation & Reasoning, Computer Vision, and Natural Language Processing. [1] In this system, it takes images and natural language as input and gives the natural language answers as output. VQA could be very helpful when it is applied to scenarios of object detections or acquisition of information. However, VQA tasks could be challenging due to the size of datasets and some other factors.

## Application
Visual Question Answering has been widely used in different real-life areas. The most direct application is to help visually impaired persons; thus, they could ask questions by just taking photos. Also, it could be used in the medical or biological field by detecting X-rays or some other medical images to tell information.
## Literature Review
A lot of VQA papers and literature reviews suggest that it would be a multi-discipline problem to combines Knowledge Representation & Reasoning, Computer Vision, and Natural Language Processing to get the final distribution of answers.
### Datasets
Images: The image dataset is from Microsoft Common Objects in Context (MS COCO) datasets[2], which has images with multiple objects and wide contextual information. [1]
Question and answers: In COCO dataset, it has already included questions and answers for each image, which are around 760,000 questions and 10,000,000 questions.
### Approaches outline in VQA
According to Antol [1], there are two channels in the model, including image channel for embedding image features and question channel for embedding question features. Convolutional Neural Network (CNN) will be used in the image channel and Long Short-Term Memory (LSTM) will be used in the question channel. Then, two features will be fused by element-wise multiplication and transformed to a fully connected layer followed by a softmax layer.
## Open-Source Research
An example of CNN&LSTM combination is the “Deeper LSTM Q + Norm I” from tbmoon Github implemented by Pytorch [3]. Also, the combination of a LSTM channel for question features and a normalized VGGNet for image features shows the best performance. The accuracies of answers are shown as follows:
