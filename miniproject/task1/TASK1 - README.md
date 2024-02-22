<h1 align="center">AZURE HANDS-ON LAB - Mini Project</h1>
<h1 align="center">Building & Running a Python Application to transform data on a Azure VM</h1>

# I. Goals

The goal is to learn the way Azure works and utilize resources within it to create a small project which will make you use and upskill you by "learn by doing"

Below are the steps detailing how to proceed in achieving this goal.

1. Create a Python Script `main.py`.
2. In the script write a method `upload_data` to read a text file [input.txt](input.txt) from your local VM instance and upload it to an `input` directory in a `data` container Azure Data Lake Gen 2 (ADLS Gen2) Storage.
3. In the same script write another method `word_count` which will now read the file that you wrote into the `input` directory and perform a word count and create a dataframe with columns `file_name`, `word` and `word_count` as the columns where `file_name` is the name of the file that was parsed, `word` is the word that is being read, `word_count` is the corresponding number of times the word has occured in the file.
4. The resultant dataframe from Step 3, must be stored back into ADLS Gen 2 storage in an `output` directory in the same `data` container. This should be done by the `save_data` method in your script `main.py`.

# II. Helper Note

For example, if `sample.txt` is the input file you are using which has the below content:

```text
Hello World
Hello
```

Then the `word_count` function would return a dataframe as follows:

<div align="center">

<table>
  <tr>
    <th>file_name</th>
    <th>word</th>
    <th>word_count</th>
  </tr>
  <tr>
    <td>sample.txt</td>
    <td>Hello</td>
    <td>2</td>
  </tr>
  <tr>
    <td>sample.txt</td>
    <td>World</td>
    <td>1</td>
  </tr>
</table>

</div>

This data is finally saved into the `output` directory of the `data` container.

Below is the high level flow diagram for reference

<div align="center">
<img src="https://github.com/Lingesh2311/GraduateLearningPlan/blob/main/miniproject/task1/HighLevelFlow.jpg" >
<p>High Level Flow diagram</p>
</div>

# III. Prerequisites & Best Practices

1. Create a free credits enabled Azure Account [More details](https://azure.microsoft.com/en-gb/free). If this is already expired, we would recommend you to create a billing strategy on a `pay-as-you-go` subscription for just a week and create a minimal configuration VM for this mini project.
2. Check for `Bs v2-series (latest generation)` or `Bas v2-series (latest generation)` windows/ubuntu VM for minimal running cost.
3. Create an Azure Data Lake Storage account (**Standard general-purpose v2**) [More details](https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal#create-a-storage-account-1)
4. Install the `Python` package in the VM and the required packages that you are using in the VM as well.
5. **Complete working solution code base in your local machine first, and test if it works, then create the VM and we can migrate the code there**
6. Installation of python packages to leverage virtual environment in Python based projects.

   - [Virtual Environment in Python - Why, What & How](https://realpython.com/python-virtual-environments-a-primer/) <br/>
   - **Commonly used packages** : [venv for Python 3.10](https://docs.python.org/3.10/library/venv.html), toggle the selection drop down for higher/lower versions, [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html)

7. A **requirements file** for your Python project. It supports **dependency management**. In short, it is a simple text file named by convention as `requirements.txt`. It is used to store the package names and the version of the python packages that needs to be installed for efficiently running a project. Below is an example:

   ```text
   requests>=2.22.0, != 2.23.0
   matplotlib==3.6.1
   ```

   **_Search & learn about requirements file, virtual environment in Python_**

   Your task in the project will be to create a `requirements.txt` file which can do the Azure based operations of reading a file from local and pushing it to cloud, and then transforming the data that was read and finally writing the output data to the cloud.

---

# IV. Miscellaneous References - Further Reading

1. [Article on Creating & Hosting Python applications in Azure VMs](https://medium.com/codex/how-to-quickly-deploy-python-apps-to-azure-vms-ba350c06a2ce)
