Optimizing an ML Pipeline in Azure

## Overview
This project is part of the Udacity Azure ML Nanodegree.
In this project, we build and optimize an Azure ML pipeline using the Python SDK and a provided Scikit-learn model.
This model is then compared to an Azure AutoML run.

## Summary
This dataset contains data about bank marketing. It has information about people's job, gender, income and more details which is represented in a table. In this project, we seek to predict which model from Azure HyperDrive ML or Azure AutoML gives us a more accurate result by maximizing the primary metric value.

The best performing model was the Azure AutoML run. It 

## Scikit-learn Pipeline
**Explain the pipeline architecture, including data, hyperparameter tuning, and classification algorithm.**

The benefits of Random Parameter Sampling is we can decide the batch size and the layer neurons and set our own 

**What are the benefits of the early stopping policy you chose?**
The early stopping or termination policy "BanditPolicy" is a conservative setting that provides approximately 25%-35% savings with no loss on primary metric. It prevents experiments from running for a long time and using up resources. It checks the job every two interations and if the primary memtric falls outside top 10%, Azure ML terminates the job.

## AutoML
**In 1-2 sentences, describe the model and hyperparameters generated by AutoML.**

## Pipeline comparison
**Compare the two models and their performance. What are the differences in accuracy? In architecture? If there was a difference, why do you think there was one?**

## Future work
**What are some areas of improvement for future experiments? Why might these improvements help the model?**

## Proof of cluster clean up
**Image of cluster marked for deletion**
