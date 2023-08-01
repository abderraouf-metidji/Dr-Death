## Dr Death

A data analysis of Dr Shipman's malpractices using:

PowerBI

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

The first dataset includes information about the confirmed victims of Dr Shipman with the following variables: 
* age
* date of death
* decision
* gender
* gender2
* name
* place of death
* year of death

The second dataset is a lot smaller and only include data that will allow a comparison between the time of death of Dr Shipman's victims and the time of death of other doctors. 

It includes:
* hour
* shipman's data
* data for comparison

What we are trying to understand with this analysis is if there is a correlation between victims mainly focusing on the type of victim (age, genre, etc.), where the death occurs (home, hospital, during surgery, etc.), and at what time does the death occur when compared to other deaths. 

---
### Data Analysis

Let's start of with a few general numbers. 

In this case there were 215 confirmed victims with an average age of 76.19.

Within these number there were a lot more women then men with 82.79% of the victims being women versus 17.21% of them being men. 

---
### Conclusion


