# Disaster-Response-Pipelines

This is project for analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages.

## Project Descriptions
The project has three componants which are:

1. [Data folder](https://github.com/aljawharah-20/Disaster-Response-Pipelines/tree/main/data) : contains the original message dataset , The script process_data.py which bulid ETL to the data and saves this to a database file.

2. [Models folder](https://github.com/aljawharah-20/Disaster-Response-Pipelines/tree/main/models) : contains the script train_classifier.py to train the model.

3. [App folder](https://github.com/aljawharah-20/Disaster-Response-Pipelines/tree/main/app) : contains the Flask webapp that categorizes new messages.

## Instructions <a name="instructions"></a>

To execute the app follow the instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`
    
3. Go to http://0.0.0.0:3001/

## Screenshots
![](https://github.com/aljawharah-20/Disaster-Response-Pipelines/blob/main/screenshots/Screen%20Shot%201442-04-23%20at%2010.42.53%20AM.png)
![](https://github.com/aljawharah-20/Disaster-Response-Pipelines/blob/main/screenshots/Screen%20Shot%201442-04-23%20at%2010.42.59%20AM.png)
![](https://github.com/aljawharah-20/Disaster-Response-Pipelines/blob/main/screenshots/Screen%20Shot%201442-04-23%20at%2010.43.03%20AM.png)

