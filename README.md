# NLP Project: Detecting Fraudulent Claims

> Python,

<!--
![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/pragyy/datascience-readme-template?include_prereleases)
![GitHub last commit](https://img.shields.io/github/last-commit/pragyy/datascience-readme-template)
![GitHub pull requests](https://img.shields.io/github/issues-pr/pragyy/datascience-readme-template)
![GitHub](https://img.shields.io/github/license/pragyy/datascience-readme-template)
![contributors](https://img.shields.io/github/contributors/pragyy/datascience-readme-template) 
![codesize](https://img.shields.io/github/languages/code-size/pragyy/datascience-readme-template) 
-->

<!-- ![img](https://github.com/bche3/AirBnB-Housing-Price-Prediction-Project/blob/main/images/airbnb-thumbnail.PNG) -->

## Project Overview

The project objective is to develop a predictive model for webpage classification based on scraping text content. A collection of unlabeled pages for you to classify has been provided. Once projects are complete we'll evaluate the accuracy of your model using the actual labels.

Preliminary tasks

1.  Augment the HTML scraping strategy so that header information is captured in addition to paragraph content. Are binary class predictions improved using logistic principal component regression?

2.  Perform a secondary tokenization of the data to obtain bigrams. Fit a logistic principal component regression model to the word-tokenized data, and then input the predicted log-odds-ratios together with some number of principal components of the bigram-tokenized data to a *second* logistic regression model. Based on the results, does it seem like the bigrams capture additional information about the claims status of a page?

3.  Build and train a neural network model. Experiment with architectures and training configurations until you find a model that performs at least as well as principal component logistic regression from task 1. Quantify the predictive accuracy.

Primary Task

1.  Develop the best predictive model you can for (a) binary classification and also for (b) the multi-class setting. You can use any preprocessing and any modeling technique you like, including ones not discussed in class (consider exploring RNN or SVM). Export a deployable copy of each model and a set of predictions from each model on the test data `claims-test.RData`. Predictions should be formatted as a single data frame named `pred_df` with columns

    -   `.id` containing the URL ID

    -   `bclass.pred` containing the predicted label for the binary class setting

    -   `mclass.pred` containing the predicted label for the multiclass setting

If this were a technical project, you might be expected to provide a *brief* executive summary of your work and a deployable version of your predictive model that could be easily used by another team or individual. In addition, you might use your model to classify new pages. Deliverables are designed to emulate these project outputs.

-   ***Deliverable 1:*** write a 1-page summary of findings for tasks 1-3; store the rendered document in the `writeups` directory.

-   ***Deliverable 2:*** write a 1-page summary of methods and findings for task 4. This should describe text preprocessing, your predictive models, and estimated prediction accuracy for each model. Store the rendered document in the `writeups` directory.

-   ***Deliverable 3:*** a set of multiclass and binary predictions on the test data, stored as `results/preds-group[N].RData` .

-   ***Deliverable 4:*** deployable copies of your fitted predictive models, stored in the `results` directory, with a short script illustrating their use to generate predictions on the test data, stored in the `scripts` directory.

*Your written summaries should be **very** high-level with a minimum of technical detail. The audience for your writeups is a project mentor or supervisor: assume the reader is familiar with the project and has a working knowledge of the methods you've used. The aim of each summary is to convey the task(s) and result(s) as simply as possible in a linear fashion: task 1, result 1; task 2, result 2; and so on. Note that your results for each task are simply a predictive accuracy (one or a few numbers) and a comment on the accuracy (generally, comparison with another result).*

## Installation and Setup
- **Technologies:**  R Studio
- **R Version:** 4.2.2
- **Packages Used:**
  - **Data Manipulation:** tidyverse, tidymodels
  - **Data Visualization:** ggplot2, yardstick, corrplot, rpart.plot
  - **Machine Learning:** randomForest, xgboost, vip, ranger, kernlab, kknn, baguette
<!-- - **General Purpose:** General purpose packages like `urllib, os, request`, and many more. -->


## Data

### Source Data
## Repository content

-   `data` contains several `.RData` files:

    -   `claims-raw.RData` contains raw HTML and class labels for 2,165 webpages

    -   `claims-test.RData` contains raw HTML for 929 unlabeled webpages

    -   `claims-clean.RData` contains cleaned data for use in training; file generated by `scripts/nlp-model-development.R` and should be replaced as preprocessing pipeline is updated

-   `scripts` contains some starter R scripts

    -   `preprocessing.R` contains *functions* for quickly ingesting raw HTML and outputting analysis-ready data; this file is intended to be sourced

    -   `nlp-model-development.R` shows example codes for preprocessing data and training a neural network and exporting the model

    -   `prediction.R` imports a trained model and generates predictions

-   `results` contains example technical outputs: a trained model and a set of predictions

-   `writeups` contains templates for written summaries
### Data Acquisition
- 

### Data Preprocessing

- 

Our variables of focus:

- `id` —
- `id` — 

## Results and Evaluation
Desc

## Future Work
Desc


<!--
## Code structure
Explain the code structure and how it is organized, including any significant files and their purposes. This will help others understand how to navigate your project and find specific components. 

Here is the basic suggested skeleton for your data science repo (you can structure your repository as needed ):

```bash
├── data
│   ├── data1.csv
│   ├── data2.csv
│   ├── cleanedData
│       ├── cleaneddata1.csv
|       └── cleaneddata2.csv
├── data_acquisition.py
├── data_preprocessing.ipynb
├── data_analysis.ipynb
├── data_modelling.ipynb
├── Img
│   ├── img1.png
│   └── Headerheader.jpg
├── LICENSE
├── README.md
└── .gitignore
```
-->

