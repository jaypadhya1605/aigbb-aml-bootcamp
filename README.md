# This is AI GBB Workshop/Bootcamp for Azure Machine Learning v2

This tutorial is an introduction to some of the most used features of the Azure Machine Learning service.  In it, you will create, register and deploy a model. This tutorial will help you become familiar with the core concepts of Azure Machine Learning and their most common usage. 

You'll learn how to run a training job on a scalable compute resource or local on premise machine,create a machine learning pipeline, we will show you how to then deploy the created model, and finally test the deployment.

You'll create a training script to handle the data preparation, train and register a model. Once you train the model, you'll *deploy* it as an *endpoint*, then call the endpoint for *inferencing*.

The steps you'll take are:

> * Set up a handle to your Azure Machine Learning workspace 
> * Create your training script
> * Create a scalable compute resource, a compute cluster 
> * Create and run a command job that will run the training script on the compute cluster, configured with the appropriate job environment
> * View the output of your training script
> * Deploy the newly-trained model as an endpoint
> * Call the Azure Machine Learning endpoint for inferencing

To Get Started start with Workshop [Setup New IPython Kernel](00_SetupIpythonKernel.ipynb)

We will follow the 

![image](https://github.com/azeltov/aigbb-aml-bootcamp/assets/5873303/e0575c72-2c32-4c83-9660-82c34993027b)

### Inner loop - Proof of concept / Model development


The inner loop element consists of your iterative data science workflow that acts within a dedicated, secure Machine Learning workspace. A typical workflow is illustrated in the diagram. It proceeds from data ingestion, exploratory data analysis, experimentation, model development and evaluation, to registration of a candidate model for production. This modular element as implemented in the MLOps v2 accelerator is agnostic and adaptable to the process your data science team uses to develop models.


### Middle loop - Scaled model training

Data science team will take advantage of hyperscale compute cluster to scale their model training.  The best models will be registered in AML model registry. After the data science team develops a model that's a candidate for deploying to production, the model can be registered in the Azure Machine Learning workspace registry. CI pipelines that are triggered, either automatically by model registration or by gated human-in-the-loop approval, promote the model and any other model dependencies to the model deployment phase.



### Outer loop - Model deployment 

The model deployment or outer loop phase consists of pre-production staging and testing, production deployment, and monitoring of model, data, and infrastructure. CD pipelines manage the promotion of the model and related assets through production, monitoring, and potential retraining, as criteria that are appropriate to your organization and use case are satisfied.



https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/machine-learning-operations-v2
