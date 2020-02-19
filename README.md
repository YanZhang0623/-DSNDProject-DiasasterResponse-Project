# Disaster Response Pipeline Project

Overview On this project, I built an ML model to help organnization classify the messages that related to disaster response. The The dataset used on this project is the Diaster Response dataset from Figure Eight.

Below are the steps I took to built the model:

* Create ETL pipeline script to clean data and convert data into proper format.
* Create ML pipeline to train and test the model by using RandomForestClassifier.
* Run Flask app to classifies the messages based on the model.

Install: This project requires Python 3.x and the following libraries installed:
  * Numpy
  * Pandas 
  * Scikit-Learn 
  * nltk 
  * Sqlalchemy 
  * re 
  * pickle

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
