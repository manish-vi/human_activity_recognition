<h1 style="text-align:center;font-size:30px;" >Human Activity Recognition</h1>

<h1> 1. Business Problem </h1>
<h2> 1.1 Description </h2>
This project is to build a model that predicts the human activities such as Walking, Walking_Upstairs, Walking_Downstairs, Sitting, Standing or Laying.
This dataset is collected from 30 persons(referred as subjects in this dataset), performing different activities with a smartphone to their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.

<h2> 1.2 Sources/Useful Links</h2>
- https://arxiv.org/pdf/1805.07020.pdf
- https://www.researchgate.net/publication/305649713_Deep_learning_for_human_activity_recognition_A_resource_efficient_implementation_on_low-power_devices

<h1>2. Machine Learning Probelm </h1>

<h2> 2.1 Data </h2>

<h3> 2.1.1 Data Overview </h3>
* Accelerometer and Gyroscope readings are taken from 30 volunteers(referred as subjects) while performing the following 6 Activities.

    1. Walking     
    2. WalkingUpstairs 
    3. WalkingDownstairs 
    4. Standing 
    5. Sitting 
    6. Lying.

* Readings are divided into a window of 2.56 seconds with 50% overlapping. 

* Accelerometer readings are divided into gravity acceleration and body acceleration readings,
  which has x,y and z components each.

* Gyroscope readings are the measure of angular velocities which has x,y and z components.

* Jerk signals are calculated for BodyAcceleration readings.

* Fourier Transforms are made on the above time readings to obtain frequency readings.

* Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.

* We get a feature vector of 561 features and these features are given in the dataset.

* Each window of readings is a datapoint of 561 features.

<h2> 2.2 Mapping the real world problem to an ML problem </h2>

<h3> 2.2.1 Type of Machine Leaning Problem </h3>
<p> It is a multi class classification problem, given a new datapoint we have to predict the Activity.</p>

## 4. Getting Started
Start by downloading the project and run "HAR_DNN_Fusion_Model.ipynb" file in ipython-notebook.

## 5. Prerequisites
You need to have installed following softwares and libraries before running this project.
1. Python 3: https://www.python.org/downloads/
2. Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy and scipy: https://www.anaconda.com/download/

## 6. Libraries
* __Gensim:__ Gensim is a Python library for topic modelling, document indexing and similarity retrieval with large corpora. Target audience is the natural language processing (NLP) and information retrieval (IR) community.
    * pip install gensim
    * conda install -c conda-forge gensim
* __Keras:__ Keras is a high-level neural networks API, written in Python and capable of running on top of TensorFlow, CNTK, or Theano.
    * pip install Keras
    * conda install -c conda-forge kera

* __xgboost:__ It is used to make xgboost regression model.
    * pip install xgboost
    * conda install -c conda-forge xgboost

* __scikit-learn:__ scikit-learn is a Python module for machine learning built on top of SciPy.
    * pip install scikit-learn
    * conda install -c conda-forge scikit-learn

* __nltk:__ The Natural Language Toolkit (NLTK) is a Python package for natural language processing. 
    * pip install nltk
    * conda install -c conda-forge nltk

## 7. Authors
•	Manish Vishwakarma - Complete work  
