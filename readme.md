

## Data

Data Fields:  

**fullVisitorIdv** - A unique identifier for each user of the Google Merchandise Store.  
**channelGrouping** - The channel via which the user came to the Store.  
**date** - The date on which the user visited the Store.  
**device** - The specifications for the device used to access the Store.  
**geoNetwork** - This section contains information about the geography of the user.  
**sessionId** - A unique identifier for this visit to the store.  
**socialEngagementType** - Engagement type, either "Socially Engaged" or "Not Socially Engaged".  
**totals** - This section contains aggregate values across the session.  
**trafficSource** - This section contains information about the Traffic Source from which the session originated.  
**visitId** - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.  
**visitNumber** - The session number for this user. If this is the first session, then this is set to 1.  
**visitStartTime** - The timestamp (expressed as POSIX time).  

Some of the data is provided in a Json format therefore the first step will be extracting and cleaning these value. 

Objectives:  

The analysis will focus on understanding the behaviour of GStore visitors using **Pandas, NumPy, Plotly and Seaborn**, answering to questions like:

- Where do visitors come from? What countries have the most buyers?
- What Operational System, Browser, Device are visitors and buyers mainly using?
- What are the most frequent channelGrouping?
- What are the most frequent Weekdays, months, days, times with the highest accesses and revenue?

After a thorough analysis I forecasted future visits to the GStore website using **fbProphet** and getting results with a MAE(mean absolute error): 165.095 as shown in the graph below.  
![image](https://user-images.githubusercontent.com/73824871/115701846-83514600-a368-11eb-8f78-408439e70fe4.png)

Finally several machine learning algorithm were applied to:  
- Classify whether future visitors would have converted into buyers.
- Predict future revenue per buyer.

The analysis has been divided into 4 notebooks to make sure they could be uploaded on Github.
All graphs are stored in the corresponding notebooks:
- [Data_extraction - 1st analysis](https://github.com/davidellavalle/Google-anayltics-customer-behaviour-and-forecast/blob/main/Data_extraction%2C_analysis_on_Geo_Network_and_devices.ipynb)
- [Analysis_on_total_and_Traffic_source](https://github.com/davidellavalle/Google-anayltics-customer-behaviour-and-forecast/blob/main/Analysis_on_total_and_Traffic_source.ipynb)
- [Merging_DFs_and_Buyer_analysis](https://github.com/davidellavalle/Google-anayltics-customer-behaviour-and-forecast/blob/main/Merging_DFs_and_Buyer_analysis.ipynb)
- [Forecast_and_M](https://github.com/davidellavalle/Google-anayltics-customer-behaviour-and-forecast/blob/main/Forecast_and_ML.ipynb)

A [folder](https://github.com/davidellavalle/Google-anayltics-customer-behaviour-and-forecast/tree/main/Presentation) with the PPTX and final presentation has been added.
