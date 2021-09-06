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

**New York City** has highest no of Deaths due to influenza which was around 6411 followed by California which accounts to 5470 deaths due to influenza. The **Texas** state has the 3rd highest deaths in U.S.A. below Pie chart as shown in Fig. 5. drawn with the help of Plotly libraries shows the same. From the Pie chart also, we can conclude the same as its clearly visible New York City Contributes 10.2 percent of the total influenza
deaths followed by California which accounts for 8.9 percent of the total deaths due to influenza.
![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Influenza%20deaths.PNG)

Illinois has the highest number of Confirmed cases with numbers exceeding more than 100 million, but has a lower number of Probable cases, whereas on the other hand Virginia with the state code VA has a large number of Probable cases close to 9 million as shown in Fig. 3.

![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Confirmed%20and%20Probable%20Cases.PNG)

We have Chosen Multi linear regression Model as we have many predictors and our intention to predict to new probable cases. We have got Adjusted R square of More than 90 percent.
![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Regression%20Model.PNG)

Increasing rise in covid-19 cases, deaths, probable cases and deaths has huge implications on the particular county, as more and more peoples get infected, the virus starts to mutate and become resistant to vaccinations. The analysis we did showed that among different states as shown in Fig. 12. , the total deaths among peoples over 65 years is highest in **California**, followed by Arizona implicating that elderly persons are more impacted by virus.

![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Total%20no%20of%20deaths.PNG)

### Conclusions
From the Analysis we can Predict that California state has maximum no of Covid 19 deaths also it has second highest death counts for various other diseases like Pneumonia and Influenza. The most interesting finding is California also accounts for maximum no of death count of elderly people of Age more than 65 years due to Covid.

# Project 2:Analysis of Time series and Logistic Regression
## Assessment of the components of the raw time series

Note:The Fig. 1. shows of raw time series data which depicts a trend with gradual increase in Trips from abroad. The Centre moving average plot removes effect of seasonality to show clear increasing Trend. The plot not only shows the trends also shows for better forecast we have to consider seasonality and trends both in this case



From September month there is gradual decrease in the number of Trips in Ireland from abroad. Also, one more interesting finding is the no of trips to Ireland is increasing from 2012 to 2019
