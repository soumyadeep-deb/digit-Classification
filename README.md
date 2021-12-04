# digit-Classification

### A deep lerning model to detect Handwritten Digits.
Dataset used: https://www.kaggle.com/c/digit-recognizer/data

I have directly fetched the dataset from kaggle, no need to upload a dataset.

To use this code, just upload your kaggle.json file, which connect Colab to the Kaggle API to fetch the dataset.

Learn more abot how to fetch data directly from kaggle: https://www.analyticsvidhya.com/blog/2021/06/how-to-load-kaggle-datasets-directly-into-google-colab/

The code is written in a modular way, i.e. using fuctions to do the stuff.

I have used **K-fold cross validation** to experiment a little bit on the number of nurons in the Dense layer.
The model with the highest accuracy was then chosen.

The training and validation, accuracy and loss curves are also plotted along with it.

The model can be tested on any test dataset, just make sure to transform your data before feeding into the model, specifications bellow:
1. Image size used: 28 x 28 x 1
2. Normalize pixel values
3. Encode your output if you haven't, (use to_categorical function)
