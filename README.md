# Disaster-Response-Pipelines

This is project for analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages.

## Project Descriptions
The project has three componants which are:

1. The folder data : contains the original message dataset , The script process_data.py which bulid ETL to the data and saves this to a database file.

2. The folder models : contains the script train_classifier.py to train the model.

3. The folder app : contains the Flask webapp that categorizes new messages.

## Instructions <a name="instructions"></a>

To execute the app follow the instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    'python run.py'

