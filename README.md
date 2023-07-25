<<<<<<< HEAD
# Chicken_Disease_Classification_Using_Deep_Learning
=======

# Chicken_Disease_Classification_Using_Deep_Learning

>>>>>>> 153d2ec40222833554dd4f2d9d203bd8b7825f0e

Steps involved in creating this project are

1. Creating template.py: template.py automatically creates all the required files and folders for the project. If any new files/folders needed to be updated or added, this can be done by modifying the template.py

2. Adding required libraries in requirements.txt

3. Updating setup.py

4. Create virtual environment

    -command for creating virtual environment

        -conda create -n 'nameofenv' python='version' -y

        here i used,

        - conda create -n chicken python=3.8 -y

        - conda activate chicken (to activate env)

        - conda deactivate chicken (to deactivate env)

5. To install requirements.txt

    -pip install -r requirements.txt

6. Creating custom log using the constructor file __init__.py in the src folder. This creates a log folder and prints the logs in the terminal as well as save the logs in the log folder for future reference.

7. Creating utils: Frequently used functions are defined in utils, so that those functions need not be called in every components again and again. Whenever needed those functions can be imported from the utils.

## Workflows

1. Update config.yaml
2. Update secrets.yaml [optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml

1. Data Ingestion:

    Data is ingested from Git repository.

2. command for viewing tensorboard

    - tensorboard --logdir artifacts/prepare_calbacks/tensorboard_log_dir/

3. commands for DVC file

    - dvc init
    - dvc repro
    - dvc dag
