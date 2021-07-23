# Sparkify

### Table of Contents

1. [Description](#description)
2. [Requirments](#requirments)
3. [Files Description](#files)
4. [Overview](#overview)
5. [Data Understanding](#data)
6. [Methodology](#method)
7. [Deploy](#deploy)
8. [Authors](#authors)
9. [Acknowledgements](#acknowledgements)


## Description <a name="descripton"></a>

This GitHub Repo represents my Capstone Project for the  Data Science Nanodegree provided by Udacity. 
We aim to use the Spark MLlib to manipulate  a large and realistic dataset, engineer relevant features  and build a machine learning for predicting churn. 


## Requirments <a name="requirments"></a>

Anaconda distribution of Python is sufficient to run the main python notebook of the project (Sparkify.ipynb), although the pyspark library (pyspark==3.1.2) might need to be installed. The main packages required to run the project outside an Anaconda distribution system are PySpark (pyspark==3.1.2), Pandas (pandas==1.3.0), Seaborn (seaborn==0.11.1), Matplotlot.pylpot (matplotlib==3.4.2). The code should run with no issues using **Python versions 3**.


## Files Description <a name="files"></a>
**Notebook**: Sparkify.ipynb

**Readme**:  Readme.md

**zip file**: A subset of the main dataset, mini_sparkify_event_data.json.zip in zip format. (NOTE: The zip file should be unziped within the directory before you run the Sparkify.ipynb notebook)

### Overview <a name="overview"></a>

Sparkify is a  fictious music streaming service like Spotify and Pandora. The data provided is the logs of every user actions of the servic as an event.
Faced with this voluminous data, we try to use PySpark, the Python API to Spark,  to analyze the users logs, built meaningful features from raw data, and build a  machine learning model to predict users who are highly likely to cancel our music service, and deploy a direct marketing  strategy by sending them special offers in order to prevent them from churning.
Our model evaluation metric is the F1 score because  precision and recall are needed at the same time as it's crucial nop to miss a great ammount of users who are likely to quit the srvices while we don't want to waste resources on users who are not likely to cancell their subscription in the music service.  Our final model reported a F1 score of 76%, which is 16% higher than sending every user marketing offers.


### Data Understanding <a name="data"></a>
For the purpose of this project, we use user log extracted from our music streaming service. The data provided contain demographic info, user activities, timestamps and etc. The full dataset is 12GB, of which you can analyze a mini subset (mini_sparkify_event_data.json) in this workspace. 


### Methodology <a name="method"></a>

For this project we had to complete several tasks:

1. **ETL**: Loading and Cleaning the data by checking for missing values that would hinder our analysis and modelling.
2. **Define customer churn**: Define a user as churned when a cancellation confirmation appears in his log data. 
3. **EDA**: Exploratory Data Analysis in order to familiarize ourselves with the data and determine our next steps in engineering meaningful features. 
4. **Preprocessing**: Pre-process the data as appropriate, e.g. convert gender column to binary numeric column, convert time related columns to human readable time stamp format.
5. **Feature Engineering**: Built meaningful features from the raw user data, which will be used to train our ML models. 
6. **Modelling**: Build models on the training data, specifically Logistic Regression, Gradient Boosted Trees, Support Vector Machines, Random Forest, and finetune and select the final model.
7. **Feature import analysis**: Investigate the importance of each feature in our model. 
8. **Evaluation** - Discussion of our model evaluation results, the selection of  the best model and suggest possible improvements. 

### Deploy <a name="deploy"></a>

The main findings of our project can be found at my [post](https://spyroula-masiala.medium.com/sparkify-a-churn-analysis-using-raw-events-and-pyspark-e62dcb0208f3) 


## Authors <a name="authors"></a>

* [Spyroula Masiala](https://github.com/Spyroula)


## Acknowledgements <a name="acknowledgements"></a>
* [Udacity](https://www.udacity.com/) for providing the Data Science Nanodegree Program

