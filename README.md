# [**Kaggle Competition: Santander Customer Transaction Prediction**](https://www.kaggle.com/c/santander-customer-transaction-prediction)

- [**Kaggle Competition: Santander Customer Transaction Prediction**](#kaggle-competition-santander-customer-transaction-prediction)
  - [**Description**](#description)
  - [**Evaluation**](#evaluation)
    - [**Submission File**](#submission-file)
  - [**Data Description**](#data-description)
    - [**How to download the Data**](#how-to-download-the-data)
  - [**Setup Python Environment**](#setup-python-environment)
  - [**Run all the cells in Jupyter Notebook**](#run-all-the-cells-in-jupyter-notebook)

<a name='description'></a>

## **Description**

At [Santander](https://www.santanderbank.com/us/personal) our mission is to help people and businesses prosper. We are always looking for ways to help our customers understand their financial health and identify which products and services might help them achieve their monetary goals.

Our data science team is continually challenging our machine learning algorithms, working with the global data science community to make sure we can more accurately identify new ways to solve our most common challenge, binary classification problems such as: is a customer satisfied? Will a customer buy this product? Can a customer pay this loan?

In this challenge, we invite Kagglers to help us identify which customers will make a specific transaction in the future, irrespective of the amount of money transacted. The data provided for this competition has the same structure as the real data we have available to solve this problem.

<a name="Evaluation"></a>

## **Evaluation**

Submissions are evaluated on [area under the ROC curve](https://en.wikipedia.org/wiki/Receiver_operating_characteristic) between the predicted probability and the observed target.

<a name="submission-file"></a>

### **Submission File**

For each Id in the test set, you must make a binary prediction of the target variable. The file should contain a header and have the following format:

```python
 ID_code,target
 test_0,0
 test_1,1
 test_2,0
 etc.
 ```

<a name="data-description"></a>

## **Data Description**

You are provided with an anonymized dataset containing numeric feature variables, the binary `target` column, and a string `ID_code` column.

The task is to predict the value of `target` column in the test set.

File descriptions
**train.csv** - the training set.
**test.csv** - the test set. The test set contains some rows which are not included in scoring.
**sample_submission.csv** - a sample submission file in the correct format.

<a name='how-to-download-the-data'></a>

### **How to download the Data**

> Get the [Kaggle API](https://www.kaggle.com/docs/api) Key to download the dataset using Kaggle API from Terminal

1. Before running the above command make sure accept the rules of the competition. Else you might see a `403 - Forbidden` error

2. Follow the commands as shown below

```bash
$ mkdir data && cd data
$ kaggle competitions download -c santander-customer-transaction-prediction
$ ls
sample_submissions.csv.zip train.csv.zip test.csv.zip
$ unzip sample_submissions.csv.zip -d sample_submissions
$ unzip train.csv.zip -d train
$ unzip test.csv.zip -d test
$ ls *
sample_submission:
sample_submission.csv

test:
test.csv

train:
train.csv
```

<a name='setup-python-environment'></a>

## **Setup Python Environment**

```python
TODO: Change the environment.yml to reflect only the conda/pip packages used in this notebook
```

```shell
$ conda env create -f environment.yml
```

<a name='run-all-the-cells-in-jupyter-notebook'></a>

## **Run all the cells in Jupyter Notebook**
