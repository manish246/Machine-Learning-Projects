# Machine-Learning-Projects

## Project 1: Analyzing Covid-19 Deaths in Patients with Different Conditions among Various Counties in the United States of America.

The Project contains different Python Notebook files as shown below:
1. x19229887_Dataset1_DAP.ipynb
2. x19229887_dataset2_dap.ipynb
3. database.ini
4. config.py
5. Joined_Datasets_Model_Buildup_Visulaization.ipynb
6. Master_Python_Notebook.ipynb

The 3rd and 4th Notebook files are "x19229887_Dataset1_DAP.ipynb" and "x19229887_dataset2_dap.ipynb" which conatined seprate datasets on which analysis has been performed individually.
1. In the both file API is being called for fetching the data.
2. Used MongoDb Atlas has been used and Codes are reproducible and for security purpose we have configuration file so that username and password are not accesible to outsiders.
3. PostgreSQL has been hosted on Microsoft Azure and for security purpose we have used Configuration file where parameters are passed so that username and password are not accessible to outsiders.

database.ini file contains Initialization parameters which will be read by config.py file which contains parameter for connection strings to connect to the PostgreSQL hosted on Azure and Mongodb Atlas. We have to import both of these files before running the python notebook files.

Joined_Datasets_Model_Buildup_Visulaization.ipynb contains the Team co-ordination task of joining different tables to get a final table and thus applying a model as well as visualizing the same.

Finally the Master_Python_Notebook.ipynb contains the code to execute the entire code suite, thus hassling away to execute the files to be run individually.

### Overview of the project:Projects Aims at finding the Total no of deaths in  united states of America due to covid and the afctor influencing it.
### Exploratory Data analysis

New York City has highest no of Deaths due to influenza which was around 6411 followed by California which accounts to 5470 deaths due to influenza. The Texas state has the 3rd highest deaths in U.S.A. below Pie chart as shown in Fig. 5. drawn with the help of Plotly libraries shows the same. From the Pie chart also, we can conclude the same as its clearly visible New York City Contributes 10.2 percent of the total influenza
deaths followed by California which accounts for 8.9 percent of the total deaths due to influenza.
![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Influenza%20deaths.PNG)
