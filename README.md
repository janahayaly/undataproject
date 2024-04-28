Name: Jana Hayaly
Pennkey: jhayaly
Hours: 9

Blurb:
    My objective for this project is to develop a framework for an interactive 
model that provides information on ESG factors. I am going to focus mainly on social and environmental data. I have two goals/portions of the project that I want to implement. The first is performing EDA on existing data and the second is visualizing that data through plotting and interactive modeling. The World Bank website allows youu to filter out and choose ESG data to put into a csv file. The data is organized by country and series, and you can access it over time. I want to process this data and use it to make predictions. For example, if I can find data sequencing how a country performed on carbon emissions over the last 25 years, I want to apply a linear regression model to predict how it will perform in the next 25 years. I want to do this for climate metrics, including waste and water. I also want to do the same for social metrics, including birth rate and women in the workforce. The package I imported for this is sklearn.linear_model, so I could use the data to train a linear regression.I actually ended up using an auto regressive model because I was modeling over time, so I imported statsmodels. I will also import numpy to allow me to plot the points and draw curves.
    The second part is to produce an interactive graphing program that allows the
client to access graphing and predictions for different ESG metrics. The way I 
see this being organized is for there to be a dropdown menu which allows you to pick which metric to assess. I allow the comparison of two countries, so there are two more dropdown menus where the client can choose what countries to compare it to. The client will then get access to a graph (line) detailing the comparison between the two and showing the progress over time for each and the prediction. For this, I will import the pandas library, as well as pyplot.

Imports:
matplotlib.pyplot
numpy
sklearn.linear_model
statsmodels.tsa.ar_model
pandas 
seaborn
ipywidgets

Class Definition:
The class I defined is a "dataframe" class that takes in a file name and reads it in as its compas attribute. There is then a getter to access that attribute, and another function to print out the compas of the dataframe.

Challenges/Changes:
One of my greatest challenges was trying to get a linear regression to work for these predictions. Switching to an auto regressive model really helped me better fit the data. Another massive issue was trying to manipulate the data set to fit the type of data that is normally passed into the linegraph plotting function. Once I found the "melt" funtion, this fell into place. Another was dealing with missing data, but finding the NaN feature and dropna function allowed me to account for that and helped a lot. One of the things I would likely change if I were to redo the project is to randomize the years which fell into the train and test data sets, because I had the most recent ones be test and that might have skewed the predictions. 

Overall, this was a fun project to work on and a great class to be in. Thank you so much and have a great summer!!!