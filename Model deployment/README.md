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

<img width="839" alt="image" src="https://user-images.githubusercontent.com/75114179/193644987-71a85c15-da40-4b97-b8be-9c31add6cae0.png">

- What we develop are machine learning models, we do so in the so-called research environment. This is an isolated environment without contact to live data when the data scientist has the freedom to try and research the different models and find out a solution to a certain product need.

- In a common setting, we have historical data and we use this data to train a machine learning model, once we're happy with the performance of our model in the research environment, we're ready to migrate it to the production environment where it can receive input from live data and output predictions that can be used to make decisions.

- We often talk about deployment of machine learning models when, in fact, we mean deployment of a machine learning pipeline.
- So what is a machine learning pipeline?
It is the series of steps that need to occur from the moment we received the data up to the moment we obtain a prediction.

- A typical machine learning pipeline includes a big proportion of feature transformation steps.

- It includes steps to train the machine learning model and steps to output a prediction.

- Why do we need to do so well, because in the live environment, we're also going to receive raw data as input and we need to transform it to create the necessary features so that the model can interpret them and return the prediction.

- When we deploy our pipeline to production, we need to do it in a way so that the pipelines are reproducible. It means that if both the pipeline in the research environment and the pipeline in the production environment receive the same raw data input, both pipelines should return this same protection, same data.

#### Reproducibility

Reproducibility is the ability to duplicate a Machine Learning model exactly such that given the same raw data as input, both models return the same output.

#### Overview of Machine Learning Pipeline

<img width="913" alt="image" src="https://user-images.githubusercontent.com/75114179/194247058-9a26f08b-4659-4e91-93f5-79096cb26459.png">

### References

- 1.*Building and Deploying a Reproducible Machine Learning Pipeline - article https://trainindata.medium.com/how-to-build-and-deploy-a-reproducible-machine-learning-pipeline-20119c0ab941*
- 2.*Building a Reproducible Machine Learning Pipeline - long article https://arxiv.org/ftp/arxiv/papers/1810/1810.04570.pdf*
- 3.*Reproducible Machine Learning - presentation, Kaggle https://www.rctatman.com/files/Tatman_2018_ReproducibleML.pdf*
- 4.*The Machine Learning Reproducibility Crisis - article, by Google developer https://petewarden.com/2018/03/19/the-machine-learning-reproducibility-crisis/*

