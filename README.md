# Disaster Response Pipeline Project

### Introduction
In this endeavor, we shall employ pre-labeled calamity messages to construct a disaster response model capable of swiftly classifying incoming messages in real-time amidst a disaster scenario. This will ensure that the messages are promptly directed to the appropriate disaster response agency.

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run the following command in the app's directory to run your web app. `python run.py`

4. Go to `http://0.0.0.0:3001/`


### Description:
1. run.py - python script to run web application.

2. Templates - web files (go.html and master.html) to run the web application.

3. process_data.py - ETL pipeline to load, clean, extract feature and store data in SQLite database

4. train_classifier.py - ML pipeline to load cleaned data, train model and save trained model as pickle
