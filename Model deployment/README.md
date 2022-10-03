## Model Deployment

#### What is Model Deployment?
The deployment of machine learning models is the process for making models available in production environments, where they can provide predictions to other software systems.

-The model deployment is challenging as it needs coordination of data scientists, IT teams, software developers and business professionals.

-Also Potential discrepancy can arise between programming language in which the model is developed and the production system language.

#### Machine Learning Pipeline

<img width="526" alt="image" src="https://user-images.githubusercontent.com/75114179/193618195-67849b69-9f88-4ba1-ac91-b7e2813233ea.png">

- Before we can use the data (raw) to train our models,  we need to carry out a lot of variable transformation, extract features from data, or create new features by combining existing ones.

- Which means along with just training the models, but we are also concerned about preprocessing the data to make it suitable to train them over. And sometimes we may not want to use all the features available to us. So we may include a type of feature selection.

- Hence, a machine learning pipeline contains a variety of steps that allow us to go from the raw data to the data format that is suitable to train the machine learning models so that we can obtain the predictions when we deploy our machine learning model, then we do not just deploy the model itself, but we needto deploy the entire pipeline. And why is that?

- Well, because both in the research and in the production environment, most likely we are going to receive the raw data.

- So we need the steps of the pipeline that will allow us to produce the mature data with which we will be able to either train the model or once the model is trained, to obtain the predictions.
