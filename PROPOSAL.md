# Data Science project proposal for Opal usage in Transportation of NSW 

## Predicting busiest and emptiest route using Opal data:

### Summary:

The Opal card travel system is governed by the transport authority of the New South Wales Government. It is an immensely prevalent travelling arrangement which is a contactless ticket collection system made accessible for the ease of public transportation services in the greater Sydney region of New South Wales, Australia.

Our group will be closely monitoring aspects like the traveller's age group, travelling time as well as other probable factors to determine and evaluate its relationship to the usage pattern. It also includes several modes of transportation as per the basis of tap-on/off events and eventually the locations nearby. What we anticipate comprising in this project will be further delineated in the section below titled as goals.


### Project Goal:

The main goals of our project are as follows:

- Number of tap-on and tap-off based on location on both daily and monthly basis using visualization techniques.
- The usage of different modes of transportation mainly buses and trains to determine busiest and emptiest routes through logistic regression model, k-means, and K nearest neighbor techniques.
- Show the relationship between which age group travelled the most based on the location using the predictive algorithm.
- Show an interactive dashboard using in depth visualization techniques and making a Jupyter notebook live on the web.

### Data Source and Background

The data set comes from open data transport for NSW.  These new open datasets are large and provide an opportunity to gain a much better understanding of how cities and regions function. 

There are 4 sets of data: -
 
1. Total no of monthly bus trips including location, Variants and count of total number of passengers. Link:- [Opal trips Bus](https://opendata.transport.nsw.gov.au/dataset/opal-trips-bus)

2. Total no of monthly train trips including location, Variants and count of total number of passengers Link:- [Opal trips train](https://opendata.transport.nsw.gov.au/dataset/opal-trips-train)

3. Total no of tap on/ tap off in a day. It includes mode of transportation, date, tap type, time and count of total number of passengers. Link: -[Opaltapon/offdaily](https://opendata.transport.nsw.gov.au/dataset/opal-tap-on-and-tap-off-release-2)

4. Total no of tap on/tap off in a particular location in a day. It includes mode of transportation, date,tap type,time,location and count of total number of passengers. Link:-  [Opal tap-on/off location](https://opendata.transport.nsw.gov.au/dataset/opal-tap-on-and-tap-off-release-2)

The file format is CSV and the data dictionary is in PDF format.


### Data cleaning

**Missing values**: There are some missing values which need to be eliminated. For example: For some data sets the postal code field has negative value (-1) which represents the null value. These data need to be eliminated.

**Data Mapping**: Some data are not meaningful, and we need to map those data with a new data set to make it meaningful. For example: Postal code is provided in the data set for the opal card, but the name of the suburb is not given. So, we need to get another dataset which contains information about postal code and suburb and map to our original data set.

**Data Grouping**: Grouping of the records to get details based on age group and city. For example: Grouping the data based on age and getting the total value of the respective age group for graphical representation and analysis.


### Techniques expected to use in the project

We expect to use a logistic regression model, k-means, and K nearest neighbor techniques to predict the busiest and emptiest places in NSW. Data visualization techniques need to be applied to show tap on and tap off data on a daily basis for understanding and gaining insight that would help to predict and come up with decisions by using libraries like Matplotlib, Seaborn, plotly, pydot.

### Project Milestones:
#### Milestone 1:
Retrieving our datasets from open data transport of NSW, loading them into data frames, and consequently joining them together. It includes cleaning our datasets, formatting rows of data, removing outliers as well as rows with NaN values. 
#### Milestone 2:
Data mapping and Data grouping is to be done to progress with the data exploration.   
Data visualization is to be carried out to show tap-on/off on an hourly basis including libraries like Matplotlib, Seaborn, Plotly, Pydot.
#### Milestone 3:
Identification of model and applying predictive algorithms like logistic regression, k- means, and K nearest neighbor techniques.
Showing an interactive dashboard and making Jupyter notebook live on the web.
