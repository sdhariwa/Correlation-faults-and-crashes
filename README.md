# A Predictive ML Model: Correlation of Faults & Crashes
This is a SOAR hackathon project for Team Phoenix.

#### Problem Statement 
The lack of correlation between system faults and crashes in CX Cloud hinders experience, necessitating a comprehensive correlation to enhance system performance. How might we prevent escalation of system issues and provide actionable insights to user?

#### Solution Proposed
The solution is provided by ideating and building a predictive ML model quoting likeliness of an asset's crash % initiating timely preventive measures from user’s end.

#### Contributing Members
- Preksha Gupta ([prekgupt@cisco.com](mailto:prekgupt@cisco.com))
- Nitish Kumar ([nitisku4@cisco.com](mailto:nitisku4@cisco.com))
- Srishti Dhariwal ([sdhariwa@cisco.com](mailto:sdhariwa@cisco.com))


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#### Notebooks In Brief

- To enhance the usability of data collected from Automated Faults Management (AFM) and Risk Mitigation Checks (RMC), the `Data Transformation.ipynb` notebook is used to convert AFM data from a text file to tabular CSV format.
- `Data Preprocessing.ipynb` addressed the unknown instances by dropping the entire column from the dataset. Data is merged using one of the common identifier, product_id.
-  In handling a dataset entirely composed of natural language, categorical columns underwent LabelEncoding to enable compatibility with Machine Learning models. To access feature relevance concerning the 'crashed' target, correlation analysis was employed. Columns exhibiting NaN correlation, indicative of zero variance, were dropped due to a lack of data variation. Few redundant columns, contributing minimally to crash determination, were also excluded. The dataset is then split in a 60:40 ratio. The implemented models include:

    1. Support Vector Regression

    2. Linear Regression

    3. Gradient Boost Regression

    4. Random Forest Regression

    5. Voting Regression with Gradient Boost, Random Forest and Linear Regression 

    6. Voting Regression with Gradient Boost, Random Forest, Linear and Support Vector Regression.

    Normalization was applied when predicted values fell outside the [0, 1] range. Evaluation metrics such as Mean Absolute Error, Mean Square Error and R-Squared Error are utilised. The `Models.ipynb` notebook executed these tasks, concluding with insightful graphical visualisations crafted using the Matplotlib package.
#### Steps to run
1. Install Anaconda:
    
    • Install Anaconda from https://www.anaconda.com/download.

2. Open Anaconda Navigator:

    • Launch the Anaconda Navigator application on your computer.

3. Launch Jupyter Notebook:

    • In Anaconda Navigator, find and click on the "Home" tab.
    
    • Locate the Jupyter Notebook icon and click on the "Launch" button.

4. Download Resources and Notebooks:
  
    • Download the data resources from [resources](https://cisco-my.sharepoint.com/:f:/r/personal/sdhariwa_cisco_com/Documents/Team%20Phoenix/resources?csf=1&web=1&e=7j9rwa) in a directory on your machine.
    
    • Download the notebooks. Make sure the notebooks and data resources are in the same directory.

5. Navigate to the downloaded Notebook:

    • The Jupyter Notebook interface will open in your default web browser.
    
    • Use the file browser to navigate to the directory where your Jupyter Notebook (.ipynb file) is located.

6. Open an Existing Notebook:
    
    • To open an existing notebook, click on the notebook's name in the file browser.

7. Execute Cells:

    • Once inside a notebook, you'll see cells. You can run a cell by selecting it and clicking the "Run" button in the toolbar, or by pressing Shift + Enter.
    
8. Stop and Restart the Kernel:
  
    • If you encounter issues or want to start afresh, you can stop and restart the kernel. Use the "Kernel" menu for these options.

9. Save and Close:
  
    • Save your work by clicking the "Save" button or using Ctrl + S (Windows/Linux) or Command + S (Mac).
  
    • Close the Jupyter Notebook tab when you are finished.

10. Shut Down Jupyter Notebook:
    
    • After you're done, go back to the Jupyter Notebook dashboard in your web browser.
    
    • Click the "Quit" button next to the running notebook to shut down the Jupyter Notebook.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Happy experimenting with more Machine Learning models 💻 

Do reach out to us via email for any suggestions and questions 📧
