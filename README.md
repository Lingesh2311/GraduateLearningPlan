# AZURE HANDS-ON LAB - Graduate Learning Plan (Python & Azure)

This is the description of the hands-on project that you will be working on. It elaborates the needs & goals that needs to be achieved by the end of the learning plan.

This goes hand-in-hand with the Learning pathway shared last week. Utilize the same as an additional study material with these hands-on task(s).

This is **NOT** going to be instruction-based rather will be based on open-ended questions. It will focus on your capability to read open source materials and apply it on an unique problem statement. This will help in building a skillset of transferring your understanding from one domain & applying the same to create **actionable insights** in another.

## Prerequisites

Below are the two (programming language + IDE) setup requirements which will be essential for your hands-on task.

1. Install Python

   You must install all the necessary tools that will be required to get hands-on with Python. The latest version of Python is 3.10.7. If you have **not** already installed Python, you can download the stable release of 3.8.10 from [here](https://www.python.org/downloads/release/python-3810/).

2. Install any one IDE

   - [VSCode](https://code.visualstudio.com/)<br/>
     _or_
   - [PyCharm](https://www.jetbrains.com/pycharm/download/#section=windows)

3. Install / Use any one Notebook based environment

   - [Jupyter Notebook](https://jupyter.org/install#jupyter-notebook)<br/>
     _or_
   - [Google Colaboratory](https://colab.research.google.com/) - Free from Google


4. Setup your [Kaggle account](https://www.kaggle.com/) - will be used to download sample datasets for tasks.

## HANDS-ON TASKS

## Understanding EDA

**Goals:**

- How to approach analyzing a simple dataset and creating insightful patterns from the data?
- What is EDA? _How can it be codified?_
- How can EDA in Python help in data munging / exploration?

**Helper resources:**

I am sharing a non-exhaustive list of resources which gives a code + descriptive walkthrough of how programmatic EDA helps customers understand meaning out of the data.

These resources will give you ideas about how to approach an EDA task and how it can help understand the data in different
shapes.

1. [Simple EDA Notebook](https://www.kaggle.com/code/alokevil/simple-eda-for-beginners/notebook)
2. [EDA Jupyter Notebook Sample](https://github.com/code4kunal/eda-with-python/blob/master/EDA%20-%20part1.ipynb)
3. [EDA Tutorial on Student Academics Performance Data Set](https://github.com/arakhia/EDA-Data-Tutorial)
4. [Legenday Titanic EDA Workflow :)](https://github.com/shivam2906/Step-by-Step-Exploratory-Data-Analysis/blob/main/Exploratory%20Data%20Analysis.ipynb)
5. [Famous Python Packages for EDA](https://blog.devgenius.io/my-3-favourite-eda-packages-in-python-d6935ad8af7c)

You are expected to **replicate** this in your own IDE / notebook environment.

Once you are comfortable replicating the above resources in your local setup, you are ready for the **challenge**!

---

## Challenge 1 : Perform EDA on a dataset which is part of the [CFI BIDA course](https://corporatefinanceinstitute.com/course/loan-default-prediction-in-machine-learning/) curriculum

#### (Take this as a challenge - don't have to take the course :))

### The ASK !

Build a python-based dashboard **notebook** which can display the relationships between the column level attributes used to predict loan defaulters.

The choice of the attributes is left for you to pick, based on your initial EDA on the dataset and exploring the data attributes from different aspects.

The data can be found [here](https://github.com/Lingesh2311/GraduateLearningPlan/blob/main/data/vehicle_loans_clean.csv.zip?raw=true), and the data dictionary [here](https://github.com/Lingesh2311/GraduateLearningPlan/blob/main/data/data_dictionary.csv)

Be explorative & come up with questions and how you can utilize this data to generate the best insights! The helper resources must help in gaining some motivation towards how to approach this dataset.

### <u>Supporting Material</u>

Concepts related to EDA can be found [here](https://www.kaggle.com/code/amritachatterjee09/eda-bank-loan-default-risk-analysis). This dates back 2 years, but can be a good start to refresh your skills on financial analysis and how to write it programmatically.

### What tools & Languages can be used for this challenge?

- IDE (Jupyter Notebooks (preferred) / Google Colaboratory / Azure Databricks)
- Programming Language (Python)
- Packages (numpy, pandas, plotly, etc.)
- I am not a fan of cheatsheets, but you can find one such [sheet](https://www.utc.fr/~jlaforet/Suppl/python-cheatsheets.pdf) for quick reference.

On top of your analysis _if_ you can create a simple dashboard in Tableau / Power BI elaborating your findings - it is a plus!

---

## Challenge 2 : Learning how flask can help build simple dashboards

Once you have completed the basic EDA on the CFI BIDA Loan default prediction dataset, you can now start building a **Web app** which can host this dashboard.

### Requirements (Wireframe)

- Landing page must allow an option to upload the dataset.
- Once the `Submit` button is pressed, it must provide the user with the dashboard (in the form of plotly plots / streamlit plots / any other package that supports dashboard-like viz.).
- The user must be able to experience a smooth UX transition.

### Resources that can help with this task / Google Search terms that can be helpful

Streamlit EDA; Flask EDA app; Basics of Flask + Python

### What tools & Languages can be used for this challenge?

- IDE (VSCode / PyCharm)
- Programming / Scripting Languages (Python, HTML, CSS)
- Packages (Flask, Streamlit, Numpy, Pandas, etc)

### Examples of Running Applications & Reference Articles

- [Sample Web app](https://dataprofessor-eda-app-app-90pqxz.streamlitapp.com/)
- [Reference Article](https://towardsdatascience.com/how-to-build-an-eda-app-in-python-af7ec4b51528)

Use this as a template and build a simple web-app that will essentially display the dashboard once the user submits a CSV file on the landing page.

---

## CHALLENGE 3: Integrating the results from Steps 1 & 2 + Hosting your solution in the cloud

Resource that we will use in Azure => **Virtual Machines**.

This will be held as part of a walkthrough session.

### Tools to Download for working with Python

1. Python (3.7)
2. IDE (VSCode or PyCharm) Community editions
3. Azure Access

---

## Recommendation :)

[Pair programming](https://en.wikipedia.org/wiki/Pair_programming#:~:text=Pair%20programming%20is%20an%20agile,two%20programmers%20switch%20roles%20frequently.) can help accelerating the strategy and is used frequently in a software development setup - Try it out as it can increase the communication bandwidth b/w the team.

---

### Miscellaneous References - Next Steps

1. [Prediction of Loan Default via Deep Learning](https://sarathi-tech.medium.com/predicting-loan-defaults-using-deep-learning-with-keras-tensorflow-78a15b196e65)

2. [Web App to Predict Loan Approval](https://medium.com/swlh/lending-club-data-web-app-ada56ff64cee)
