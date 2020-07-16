# Disaster Response Pipeline Project

### Project Summary:
	This project is uses data given by Figure Eight to simulate an ETL, NLP and ML pipeline. We take in Crisis message data and 
    category data, turn these csv files into a usable format and tokenize all the message data. From there we create an ML pipeline
    to be able to predict the correct disaster recovery response by diaster agency. All together, this model becomes part of an API
    for a Web Application done using Flask
    
### Inclusions:

 - The app Folder contains files related to the web application
 - The data folder contains files related to the ETL pipeline
 - The models folder contains files related to the NLP/ML pipeline

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://127.0.0.1:5000/
