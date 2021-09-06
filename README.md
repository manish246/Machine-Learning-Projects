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

# Project 2:Analysis of Time series and Logistic Regression using R
## Assessment of the components of the raw time series
The Project contains different Python Notebook files as shown below:
1. Arima Model.R
2. Holt_model.R
3. Holt_winter_model.R
4. Naive model.R
5. SES model.R
6. R file with pCA.R


Note:The Fig. 1. shows of raw time series data which depicts a trend with gradual increase in Trips from abroad. The Centre moving average plot removes effect of seasonality to show clear increasing Trend. The plot not only shows the trends also shows for better forecast we have to consider seasonality and trends both in this case
  ![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/Trends.PNG)


From September month there is gradual decrease in the number of Trips in Ireland from abroad. Also, one more interesting finding is the no of trips to Ireland is increasing from 2012 to 2019.
![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/seasonal%20Plots.PNG)

## SIMPLE EXPONENTIAL SMOOTHENING
The first model which we have implemented is simple smoothening model (SES) in our Overseas Trips Dataset. The SES is used where there is no trend or no season effect, but as discussed above we have both trends and season present in our dataset.first we have to remove that for that we have first find out the order of differencing in Training set which can be find out by ndiff function.
We have to find the minimum value for smoothening parameter in our model for which we have used loop. We are passing the value of alpha from 0.01 to 0.99 to get the value of alpha at minimum RMSE The value of alpha which we got from the loop is 0.01 and a minimum RMSE of 734.We have also plotted graph Minimum alpha at minimum RMSE. The Fig. 6. Shows the same in which we can see that we are getting alpha as 0.01 at 734 RMSE
![](https://github.com/manish246/Machine-Learning-Projects/blob/main/Images%20for%20Data%20analysis%20Performed%20on%20Covid-19%20Datasets/SES.PNG)
