# Stroke-Prediction-with-TensorFlow-Extended
## Why MLOps?

Industry Data Science has diverged into a few dominant verticals as the field has matured, but the primary specialty has been Enterprise Machine Learning (with Product-centric Data Science as a close second). The realm of Enterprise Machine Learning, so far, has looked quite similar to how Kaggle looks — hacky ML notebooks that get the job done for a short duration of time on a specific task (sometimes with a small team, but the scope of impact is relatively minor).

In recent years, Data/AI roles and projects have gotten large budgets to bring about the promised holy grail of value each organization is looking for. Unfortunately, the industry is still lacking in fully realizing the value of most of its investments in AI, considering how few notebooks actually end up in production (and work). The field has recently delved headfirst into the world of MLOps to deal with this massive impediment.

MLOps, or Machine Learning Operations, is a set of tools, practices, techniques, and cultures that ensure reliable and scalable deployment of machine learning systems. Most Enterprise ML projects rarely make it past Level 0, limiting the business’s ability to realize true value and keeping ML projects in sandbox mode in perpetuity. This post will clarify the differences between Level 0 and Level 1 and suggest how we can get to a more advanced stage of MLOps maturity.

## Getting Started

The dataset was downloaded from Kaggle here: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

In a real MLOps infrastructure, this will likely not be a CSV but instead a table in a data warehouse or an API connection to stream data in.

The first notebook to start with is schema_curation.ipynb which walks through the initial reading and cleaning of the dataset and creating the schema to validate new data in with.

Then the pipeline goes as such:
1. data_validation.ipynb
2. data_preprocessing.ipynb
3. data_modeling.ipynb

The reason for this separation is to simulate a real world, collaborative scenario where you likely will need to save inputs and outputs out in various locations and also have an easier time to build in triggers and checks.
