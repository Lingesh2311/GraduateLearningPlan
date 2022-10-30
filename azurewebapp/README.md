<h1 align="center">AZURE HANDS-ON LAB - Graduate Learning Plan</h1>
<h1 align="center">Building & Hosting an Azure Web App on Azure Cloud</h1>

Now that you have achieved the goal of creating a web application locally, it is time to push the same to the cloud so that users outside/within the organization can access it from a public IP address via the internet. The Azure plane sees to that the application code is secured and developers can keep working on their own copies locally, until they feel a newer version needs to replace the one hosted on Azure.

## Goals

This challenge is a segue from the previous task of working on building an EDA based web app using python + streamlit / flask framework.

- We are trying to host your web app onto the Azure ecosystem, so clients can access it from the internet.
- Once the solution is hosted, we can think in lines of maintaining different versions using **Git** version control.

Below are the steps detailing how to proceed in achieving this goal.

## Prerequisites

1. Complete working solution code base in your local machine.

2. Running Solution is secured with username/password combination, so as to prevent solution leaks.

3. Installation of python packages to leverage virtual environment in Python based projects.

   - [Virtual Environment in Python - Why, What & How](https://realpython.com/python-virtual-environments-a-primer/) <br/>
   - **Commonly used packages** : [venv for Python 3.8](https://docs.python.org/3.8/library/venv.html), toggle the selection drop down for higher/lower versions, [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html)

4. A **requirements file** for your Python project. It supports **dependency management**. In short, it is a simple text file named by convention as `requirements.txt`. It is used to store the package names and the version of the python packages that needs to be installed for efficiently running a project. Below is an example:

   ```text
   requests>=2.22.0, != 2.23.0
   matplotlib==3.6.1
   ```

   **_Search & learn about requirements file, virtual environment in Python_**

5. Access to Azure resources - _will be provided_

## CHALLENGE 3: Integrating the results from [Challenges 1 & 2](README.md#challenge-1--perform-eda-on-a-dataset-which-is-part-of-the-cfi-bida-course-curriculum) + Hosting your solution on Azure cloud

Resource that you will use in Azure => **Virtual Machines** &/ **Azure Web Apps**

There are many ways of completing this task. I am listing down two of the ways I have encountered/used:

1. Via existing templates & Azure Web App Service

   One direct and a fast way if you have developed a flask-based web app or Django-based web app is to leverage the templates given by Microsoft itself.

   This [flask template project](https://github.com/Azure-Samples/msdocs-python-flask-webapp-quickstart) / [Django template project](https://github.com/Azure-Samples/msdocs-python-django-webapp-quickstart) and the [steps](https://learn.microsoft.com/en-us/azure/app-service/quickstart-python?tabs=flask%2Cwindows%2Cazure-cli%2Cvscode-deploy%2Cdeploy-instructions-azportal%2Cterminal-bash%2Cdeploy-instructions-zip-azcli) can help in providing you with a skeleton logic to host your web app in the cloud.

2. Via Azure VMs & no other resources

   Another way is to just use the Azure VM to host your solution. This is succintly explained in this [article](https://imsabirpiludiya.medium.com/deploy-python-flask-app-in-azure-vm-using-azure-devops-organization-pipeline-27e41929e5f0) and it is a quick setup for situations that don't need any hassle in terms of spending more money / setting up a dedicated Azure web-app service for hosting your solution.

### Recommended Training

1. Azure AZ-900 Learning Path : Modules [1](https://learn.microsoft.com/en-us/training/paths/microsoft-azure-fundamentals-describe-cloud-concepts/), [2](https://learn.microsoft.com/en-us/training/paths/azure-fundamentals-describe-azure-architecture-services/), [3](https://learn.microsoft.com/en-us/training/paths/describe-azure-management-governance/)
2. First three modules in this learning path [Intro to Azure VMs & building a web app with it](https://learn.microsoft.com/en-us/training/paths/deploy-a-website-with-azure-virtual-machines/)

---

### Miscellaneous References - Further Reading

1. [MEAN Stack for deploying full-fledged apps with multiple technologies on Azure VMs](https://learn.microsoft.com/en-us/training/modules/build-a-web-app-with-mean-on-a-linux-vm/)

2. [Microsoft Learn - Hosting web app with Azure App service](https://learn.microsoft.com/en-us/training/modules/host-a-web-app-with-azure-app-service/)
