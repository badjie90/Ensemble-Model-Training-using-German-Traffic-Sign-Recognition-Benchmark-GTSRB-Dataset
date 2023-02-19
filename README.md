### Ensemble-Model-Training-using-German-Traffic-Sign-Recognition-Benchmark-GTSRB-Dataset

In this repository, you can find a comprehensive deep learning multi-class classification project that leverages the power of the ensemble method to combine multiple models for superior performance. The code is openly available for anyone interested in gaining a deeper understanding of how to integrate different deep learning models to tackle various machine learning tasks with ease.

By utilizing this code, you will have the opportunity to explore and experiment with different ensemble techniques that can be employed to improve the accuracy and efficiency of your machine learning models. Moreover, you will gain valuable insights into the best practices for creating complex models, including feature engineering, hyperparameter tuning, and model selection.

As a courtesy, we kindly request that you acknowledge the original author of this code if you choose to use it for your own project. We believe that sharing knowledge and resources is essential for the growth and development of the machine learning community, and we appreciate your support. Thank you for your interest in this project, and we look forward to seeing the incredible results you will achieve with it.


The dataset used in this project is an open source dataset and can be found at: [Link]( https://sid.erda.dk/public/archives/daaeac0d7ce1152aea9b61d9f1e19370/published-archive.html)



## Steps to convert the data into pickle file.

### To download dataset:

run the following command in the project directory

$ ./downloadDataset.sh 
This will download the zip file and unzip in the current directory as GTSRB. The data formatting of images is given in Readme-Images.txt

To generate pickle files using GTSRB dataset
change the parameters according to the requirement

dataGen = datasetGenerator(nClasses=5, nTrainSamples=800, nTestSamples=100, nValidateSamples=100,imageSize=[28, 28])

nClasses - no of classes
nTrainSamples - no of Training samples
nTestSamples - no of test samples
nValidateSamples - no of validation samples
imageSize - size of 2D image matrix to be resized into.
$ python datasetGenerator.py

This will generate the following files

├── info.txt

├── test.p

├── train.p

└── validate.p













## Importance of ensemble model training

Ensemble model training is a powerful technique for improving the performance of image classification tasks in the context of deep learning. It involves training multiple models and combining their outputs to obtain better predictions than any individual model could achieve alone.

Here are some reasons why ensemble model training is important for image classification tasks in deep learning:

1. Increased accuracy: Ensemble models can improve accuracy by combining the strengths of multiple models. Each individual model may make different errors, but the combination of models can reduce overall error rates and improve accuracy.

2. Robustness: Ensemble models can be more robust to changes in the input data or to changes in the model itself. For example, if one model is overfitting to the training data, the ensemble can still make accurate predictions by relying on the other models.

3. Diversity: Ensemble models can benefit from the diversity of the models used. By training different models with different architectures, initializations, and hyperparameters, an ensemble can leverage a range of approaches to improve performance.

4. Generalization: Ensemble models can help to generalize better to new, unseen data by reducing the impact of individual model biases and overfitting to the training data.

In essence, ensemble model training is an important technique for improving the performance and robustness of image classification tasks in deep learning. It can help to achieve state-of-the-art results and is widely used in many real-world applications.
