# american-sign-language-cv

The American SIgn Language is designed to assist the deaf and hard of hearing
community to convey using hand gestures in the United States of America. In this repo I have developed
a Machine Learning solution to translate the American Sign Language into English. 
I have explored a few different machine learning models such
as Resnets, VGG Networks, DenseNets and a few other models. These are some of the
most commonly used CNN architectures used for various Computer Vision Tasks. Our
objective here was to understand how these different models perform with this data and
propose the most suitable CNN architecture.

## Dataset
The dataset from kaggle consists of 87,000 images, each of size 200x200. This dataset has
been split such that each of the 29 classes have about 3000 images per class. Along with this
the test dataset consists of 29 images, one for each class.

The test data is insufficient to accurately determine the performance of any model built.
Thus, to overcome this, I have found another dataset hosted on Kaggle called the “ASL
Alphabet Test”. This dataset contains 870 images each of size 200x200. So I intend to use the
original dataset for training and validation, and the new dataset for testing.


## Results

Among the various deep learning networks have experimented with, ResNet is performing
well on given test and train sets, so used this model to test on external images. Although
ResNet18 is able to capture patterns on the given data, the external images contain diverse and
merging backgrounds, which makes it difficult to test on these images when
compared to images with the same/ uniform background. I have achieved 70% accuracy in
the mentioned external dataset. Below is the performance of models built in
this project in terms of accuracy score

Model         Validation   Test 
AlexNet       94.1         79.2
VGG16         89.9         78.5
DenseNet121   91.1         75.8
ResNet18      99.8         89.3
