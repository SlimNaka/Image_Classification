# Image_Classification: Japanese Calligraphy

## Authors:
Sean Nakagomi, instructed by Dr. Galen Egan

## Requirements:
This project was created using Python via Google Colab.

## Introduction:
Thanks to my old man not wanting to teach me his native language when I was a young child, my Japanese sucks. Reading is especially difficult and when reading handwritten characters, especially calligraphy, I'm practically illiterate.

In this notebook, I will use the KMNIST dataset to see if we can differentiate between various hiragana characters in calligraphy.

## Data:
The data is from one of TensorFlow's built-in datasets: KMNIST.

This dataset is a replacement for the MNIST dataset (28x28 grayscale, 70,000 images), but due to the restriction of 10 classes (or labels), we have the following characters representing each of the 10 rows of Hiragana: お, き, す, つ, な, は, ま, や, れ, and を.

## Data analysis: Sean_Nakagomi_Image_Classification.ipynb
We first uploaded the data, splitting it into the predetermined train and test sets, and included all information and labels.

We checked the shape and viewed a sample of each of the ten images.

For preprocessing, we flattened all images into a 1D array and normalized them, maintaining the train and test set and their labels.

We then created a neural network with adjustable values that affect the accuracy and speed of the model.

We passed the preprocessed images through the neural network multiple times, changing the combination of adjustable numbers each time, tracking and saving each sweep. The most accurate trial number is noted each time and is used to show the accuracy of the model and then visualized by generating a confusion matrix.

We finish with a discussion of the results and a brief recap of the notebook as a whole.

## Licence:
MIT License

Copyright (c) 2024 Sean Nakagomi

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
