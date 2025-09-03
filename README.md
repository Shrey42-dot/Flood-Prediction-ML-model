This is a ***Flood Prediction*** machine learning model based on several environmental factors.
This project demostrates data processing, model training, evaluation and prediction using **supervised learning** approach..

Floods are a great force of nature and can be greatly devastating when they are not predicted earlier. Prediction of floods can reduce the loss of life and materials which we have seen a lot in most of the cases of floods. 
This project aims to solve this problem.. 

This is a very basic flood prediction model, in this project:
    -Data used was from ***Kaggle***.
    -Data was analyed and preprocessed.
    -Multiple ML models were trained and compared.
    -The best performing model was for prediction. 

The Project Steps:

    Followed these steps systematicaly:
    1_ Load and explore dataset.
    2) Perform EDA (Exploratory Data Analysis).
    3) Apply Feature Engineering.
    4) Train baseline models (Random Forest, XGBoost).
    5) Perform Hyperparameter Tuning.
    6) Evaluate & visualize results.
    7) Draw conclusions & future improvements.

This is the Kaggle Dataset CSV file -- https://drive.google.com/file/d/1HnnNeKe06y-qJoREP5A43QtvOpbiDORH/view?usp=sharing

Feature engineering was used to create new features that can be more useful that the features aready given in the dataset..

The Features present in the original dataset were -- 

    'MonsoonIntensity', 'TopographyDrainage', 'RiverManagement', 'Deforestation', 'Urbanization', 'ClimateChange', 
    'DamsQuality','Siltation', 'AgriculturalPractices', 'Encroachments', 'IneffectiveDisasterPreparedness',  
    'DrainageSystems', 'CoastalVulnerability', 'Landslides', 'Watersheds', 'DeterioratingInfrastructure', 'PopulationScore',
    'WetlandLoss', 'InadequatePlanning', 'PoliticalFactors', 'FloodProbability'
    
with the total of 21 columns out of which 'FloodProbability' was used as the target data entry..

The Features added after applying ***feature engineering*** are -- 

    --Rainfall × Deforestation
    --River Management × Dam Quality
    --Urbanization × Inadequate Planning
    --Climate Change × Coastal Vulnerability
    --Climate Change × Wetland Loss

80% of the dataset was used for training of the model and 20% was used for testing..

Two ***regression*** model were used namely 
    --RandomForest regressor 
    --XGBoost Regressor
The ***Evaluated score*** based on the ***R2 evaluation*** of both models were: 
    --Random Forest R2: 0.7630664024594073
    --XGBoost R2: 0.9385636739308599


***Hyperparameter Tuning*** was done only on the RandomForest using the RnadomisedSearchCV to find the best parameters meanwhile 
the ***Cross Validaton*** was done only on XGBoost R2 score, the mean R2 score thus found of the ***XGBoost result*** was: 
0.9840210306048119


The final Visulation was done on four different graphs to determine the accuracy of the model thus created with the actual Flood Prediction score in the original dataset 
The Graphs showed that the predicted values were very close to the actual results so the accuracy of the model was found to be ***satisfactory***. 

The following graph will give a clear picture of the accuracy of the model :


<img width="545" height="547" alt="image" src="https://github.com/user-attachments/assets/34474bcf-8c9f-4f8b-852d-f80f5e87a2f0" />
.

<img width="545" height="547" alt="image" src="https://github.com/user-attachments/assets/92ac8478-39a7-41da-9259-969c43e7cf14" />



The Teach stack used are--
  Python 
  Scikit-learn
  Pandas/Numpy
  Matplotlib/Seaborn
  XGBoost 
  

To requirements are
  
    numpy>=1.21.0
    pandas>=1.3.0
    scikit-learn>=1.0
    matplotlib>=3.4.0
    seaborn>=0.11.0
    xgboost>=1.5.0
  
They are also given in requirements.txt file. To install the requirements file just run -- 

    pip install -r requirements.txt
    

My personal details are 

  ***GitHub***: https://github.com/Shrey42-dot
  
  ***LinkedIn***: www.linkedin.com/in/shrey-pandey-





