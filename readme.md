## Dr Death

A data analysis of Shipman's malpractices using:

![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

### Power BI Tool Overview: What is Power BI, What is a Dashboard, Advantages and Disadvantages, Key Features, Data Sources, and Visualizations.

1.  What is Power BI? Power BI is a business intelligence (BI) tool developed by Microsoft. It allows users to connect, analyze, and visualize their data in the form of interactive reports and dynamic dashboards. Power BI offers a suite of tools, including a desktop application, an online version (Power BI Service), and mobile apps for Android and iOS.
    
2.  What is a Dashboard? A Dashboard is a visual representation of data that enables users to monitor and analyze essential information concisely and comprehensibly. It combines different charts, tables, maps, and other visual elements to provide an overview of key performance metrics or specific indicators.
    
3.  Advantages of Power BI:
    
    -   User-Friendly: Power BI offers a user-friendly interface with drag-and-drop features, making the creation of reports and dashboards intuitive.
    -   Broad Connectivity: It provides a wide range of connectors to connect to different data sources, including databases, flat files, cloud services, etc.
    -   Real-Time Analysis: Power BI allows real-time analysis by automatically refreshing data at defined intervals.
    -   Collaboration and Sharing: Users can share their interactive reports with other members of the organization, promoting collaboration.
    -   Integration with Microsoft Ecosystem: Power BI integrates tightly with other Microsoft tools like Excel, Azure, SharePoint, etc.
4.  Disadvantages of Power BI:
    
    -   Expensive Licenses: Advanced features of Power BI require paid licenses, which can be a drawback for small businesses with limited budgets.
    -   Processing Limits: In some situations, Power BI may be less performant when processing very large data volumes.
    -   Internet Dependency: Using Power BI Service (online) requires an internet connection, which can be inconvenient in areas with limited connectivity.
5.  Key Features of Power BI:
    
    -   Interactive Report Creation: Power BI enables the creation of visually appealing reports with a variety of visualizations.
    -   Dynamic Dashboards: Users can assemble interactive dashboards with customizable elements.
    -   Advanced Data Analysis: The tool offers powerful analysis features, such as Data Analysis Expressions (DAX) measures and calculated columns.
    -   Collaboration and Sharing: Power BI facilitates collaboration by allowing sharing of reports and dashboards with other users.
    -   Data Integration: It provides connectors to connect to various data sources, both on-premises and in the cloud.
6.  Supported Data Sources for Power BI:
    
    -   Relational Databases: SQL Server, MySQL, Oracle, etc.
    -   Cloud Services: Azure SQL Database, Azure Data Lake Storage, Amazon Redshift, Google BigQuery, etc.
    -   Flat Files: Excel, CSV, XML, etc.
    -   Web Services: REST API, OData, JSON, etc.
    -   Applications: Salesforce, Google Analytics, Microsoft Dynamics 365, etc.
7.  Visualizations Available in Power BI: Power BI offers a wide range of visualizations to represent data, including:
    
    -   Charts: lines, columns, areas, bars, pies, etc.
    -   Geographic Maps: choropleth maps, bubble maps, etc.
    -   Tables: interactive data tables.
    -   Diagrams: organizational charts, spider charts, etc.
    -   Maps: custom maps and layouts.

Power BI is a versatile tool that helps businesses turn data into actionable insights for decision-making. Its ability to connect to multiple data sources, user-friendliness, and real-time analysis capabilities make it a popular choice for many organizations. However, it's essential to consider the associated license costs and specific data processing requirements to assess its suitability for a given business.

---

### Data Context and Studied problem

For this data analysis we were given two different datasets. 

The first dataset includes information about the confirmed victims of Shipman with the following variables: 
* age
* date of death
* decision
* gender
* gender2
* name
* place of death
* year of death

The second dataset is a lot smaller and only include data that will allow a comparison between the time of death of Shipman's victims and the time of death of other doctors. 

It includes:
* hour
* shipman's data
* data for comparison

What we are trying to understand with this analysis is if there is a correlation between victims mainly focusing on the type of victim (age, genre, etc.), where the death occurs (home, hospital, during surgery, etc.), and at what time does the death occur when compared to other deaths. 

---
### Data Analysis

Let's start of with a few general numbers. 

In this case there were 215 confirmed victims with an average age of 76.19 (75.97 for women and 77.24 for men).


Within these number there were a lot more women then men with 82.79% of the victims being women versus 17.21% of them being men. This gives us 37 men killed and 178 women killed.

![Alt text](/../<images>/path/to/percentage_of_deaths_by_gender.png?raw=true "Deaths by Gender")

This means that Shipman's victims were mainly women and it was his main focus. We have almost 5 dead women for 1 man. 

Regarding the place of death we can see with the following graph that a vast majority, 204 out of the 215 confirmed victims, died in their own home. 

![Alt text](/../<images>/path/to/number_of_deaths_by_place_of_death.png?raw=true "Place of Death")

This would simply mean that their death should be categorized as "natural causes" but knowing the case this means that they were poisoned and then died when they arrived home or shortly after due to an overdose. 

When looking at the year of deaths of the patients. 

![Alt text](/images/number_of_deaths_by_year_of_death.png "Year of Death")

We can see that Shipman was the most active 1997 with a total of 37 victims that year. We can also see a small pattern reagrding his activity with and increase of deaths, a slower period, a bigger increase, slow period again, and another bigger increase. 

Here is what it looks like with the numbers:
* 1975: 1
* 1978: 4
* 1979: 2
* 1985: 11
* 1989: 12
* 1992: 1
* 1993: 16
* 1994: 11
* 1997: 37
* 1998: 18

We can see that we was more or less careful at the beginning by allowing a timeframe with close to no deaths but later on in his career he increased his killing count quite substentially. 

Now, let's take a look at the time of death of Shipman's victims compared to "normal" time of deaths. 

![Alt text](/../<images>/path/to/other_doctors_patients_and_shipman_patients_by_hour_of_death.png?raw=true "Time of Death")

The main thing that we can notice with this comparison is that the number of deaths in Shipman's case were a lot higher compared to other Doctors deaths. 

The other main thing that we can notice is that there is a huge gap between death from 1:00pm to 3:00pm when comparing the data. 

* 9.00 vs 3.80
* 14.10 vs 2.00
* 13.00 vs 3.40

This means that Shipman victims died mostly in the early afternoon whereas other doctors deaths occured at random times with the second lowest point being at Shipman's second highest, at 2:00pm. 

This shows that Shipman's patients deaths did not occur naturally since we have a specific range of the time when death occured that is not in accordance with other doctors data.

---
### Conclusion

What we have seen with the data analysis allows us to answer the question we asked ourselves at the beginning: What types of people did Harold Shipman murder, and when did they die?

We have been able to see that Shipman murdered mainly women, 178 of them, with an average age of 75.97. He also did kill men, 37 of them, with a higher average age of 77.24.

Regarding when they died we were able to notice that they mainly died in their own homes, 204 out of 215 and during the early afternoon from 1:00pm to 3:00pm. 

But, this doesn't mean that other victims didn't die at other time of day. The number of victims is so high that deaths occured at every hour of the day throughout the years.

In conclusion, he mainly killed older women, who died in their own home and most likely in the early afternoon. 
