# Disaster Response Pipeline Project

### Objective:
This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. The dataset contains pre-labelled tweet and messages from real-life disaster events. The project aim is to build a Natural Language Processing (NLP) model to categorize messages on a real time basis.

It has 3 sections:
1. Building an ETL pipeline to extract data, clean the data and save the data in a SQLite Database
2. Building a ML pipeline to train our model
3. Run a Web App to show our model results

![Web App](https://github.com/Saby-11/Disaster_Response_Pipelines/blob/master/Web_App.png?raw=true)

### Installations:
1. Python 3+
2. ML Libraries: NumPy,  Pandas, SciPy, SkLearn
3. NLP Libraries: NLTK
4. SQLlite Libraries: SQLalchemy
5. Model Loading and Saving Library: Pickle
6. Web App and Visualization: Flask, Plotly

### File Contents:
``` Disaster_Response_Pipelines <br/>
          |-- app <br/>
                |-- templates<br/>
                        |-- go.html<br/>
                        |-- master.html<br/>
                |-- run.py<br/>
          |-- data
                |-- disaster_message.csv
                |-- disaster_categories.csv
                |-- DisasterResponse.db
                |-- process_data.py
          |-- models
                |-- classifier.pkl
                |-- train_classifier.py
          |-- Pipelines
                |-- categories.csv
                |-- ETL Pipeline Preparation.ipynb
                |-- ETL_preparation.db
                |-- messages.csv
                |-- ML Pipeline Preparation.ipynb
          |-- README 
```
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

#### Note: Pipelines Folder is not essential to run the Web App.

### Acknowledgements:
1. [Udacity](www.udacity.com) for this Data Science Nanodegree Program.
2. [Figure-Eight](www.figure-eight.com) for the relevant dataset.
