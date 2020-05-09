# Disaster Response Pipeline Project

### Objecctive:
This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. The dataset contains pre-labelled tweet and messages from real-life disaster events. The project aim is to build a Natural Language Processing (NLP) model to categorize messages on a real time basis.

It has 3 sections:
1. Building an ETL pipeline to extract data, clean the data and save the data in a SQLite Database
2. Building a ML pipeline to train our model
3. Run a Web App to show our model results


### Installations:
1. Python 3+
2. ML Libraries: NumPy,  Pandas, SciPy, SkLearn
3. NLP Libraries: NLTK
4. SQLlite Libraries: SQLalchemy
5. Model Loading and Saving Library: Pickle
6. Web App and Visualization: Flask, Plotly

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
