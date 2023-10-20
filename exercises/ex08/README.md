# Exercise 08 - Creating the View & Analytic Model

> :memo: **Note:** This is part of the <strong>Fast Track</strong> and a mandatory exercise.

---
## :beginner: Detour: SAP Datasphere - Views & Analytic Models

A View in SAP Datasphere provides you with several benefits:
- Graphical or script-based editor
- Define views on top of remote, replicated data sources, or tables
- Define unions and joins, rename and remove columns, add calculations and filters
- Create Fact, Dimensions or Relational Datasets
- Create Parent-Child or Level-based hierarchies in Dimension views
- Define measures & attributes in Fact
- In the Graphical View Builder, you can compute and display the corresponding SQL Statement
<br>  

A View in SAP Datasphere allows you to leverage local tables, remote tables, or views and combine
those into a new View. A View can also contain additional elements, such as filters and calculated columns and
a view is consumable in SAP Analytics Cloud.
<br>  
An Analytic Model in SAP Datasphere provides you with several benefits:
- Rich measure modelling
- Create very complex calculation models and even refine them in SAP Analytics Cloud
- Collection of user input via prompts in SAP Analytics Cloud
- Data previewing
- Time-dependency support
- Dependency Management & Transport
<br> 

Analytic models are the analytical foundation for making data ready for consumption in SAP Analytics Cloud. They allow you to create and define multi-dimensional models to provide data for analytical purposes to answer different business questions. Pre-defined measures, hierarchies, filters, parameters, and associations provide flexible and simple navigation through the underlying data.

## End of Detour

## Start of the exercise
In this exercise, we will create our first view based on our previously created tables into an asset in SAP Datasphere, which then can be consumed in SAP Analytics Cloud.

1. Log On to your SAP Datasphere tenant.
2. Select the menu option Data Builder on the left-hand side.
3. Click New Graphical View.
<br>![](images/00_00_0071.png)  
  
4. On the left-hand side you can decide between:<br><ul><li>Repository: Here you have access to the local tables (imported data), Views, Intelligent Lookups and Shared Objects.</li><li>Sources: Here you have access to tables and views from your connections.</li></ul>

5. Ensure you select the option Repository.
6. Open the list of Tables. 
7. You are presented with the list of tables, which we created previously.
<br>![](images/00_00_0083.png)  
  
8. Drag and Drop the table Sales Transactions to the canvas.
9. You automatically will – in addition to the table you dragged to the canvas – receive the output view as well,
in our example called View 1.
<br>![](images/00_00_0084.png)   
  
10. Ensure the option Details (top right corner) is enabled. Otherwise, click on the output view that was added, in our example View 1.
11. Navigate to the Properties window.
<br>![](images/00_00_0086.png) 

12. Here you can configure Properties for the final output:<br><ul><li>You can configure the Business Name as well as the Technical Name.</li><li>You can configure the Type of Dataset.</li><li>You can decide if the View can be consumed or not.</li><li>You can choose which of the available Columns are shown or will be hidden.</li><li>You can define additional Associations.</li><li>You can provide details on the Business Purpose, which then will be available as part of the
Business Catalog.</li></ul>
13. Enter ***Sales View – Fact*** as Business Name.
14. The Technical Name will be generated based on the Business Name, but you can also change it and enter ***Sales_View__Fact***.
15. Set the semantic Usage to the ***Fact*** option.
<br>![](images/00_00_0082.png)   
  
16. Enable the option Expose for Consumption.
<br>![](images/00_00_0882.png)   
  
17. In the panel on the right hand side, scroll down to the Attributes section.
18. Now open the context menu for the Attribute ***Profit***
19. Select the option Change to Measure.
<br>![](images/00_00_0087.png)  
  
20. Repeat the steps for the Attributes ***Discount***, ***Revenue***, and ***Cost***.
21. Scroll down to the Associations.
22. Click the “+” sign to add a new Association.
<br>![](images/00_00_0088.png) 
  
23. Select the option Association.
24. You are being presented with the list of Tables and Views from your Space.
25. Select the entry for TABLE ***Product*** [Local Table (Dimension)].
26. Click ***OK***.
<br>![](images/00_00_0089.png)   

27. Ensure the Association is based on the column Product ID in both tables. In case the Association is not
suggested or is defined on another column, you can delete the join and use a simple drag and drop motion
to define a new one.
<br>![](images/00_00_0886.png)  

28. In the Details panel, click on the “Sales View - Fact” option to navigate back to the main Properties window.
<br>![](images/00_00_0887.png)  

> :boom: ***Important*** :boom: <br> 
> 29. You can now continue and repeat the steps 24 - 28 for the other associations:<br>- TABLE: Sales Manager [Local Table (Dimension)]<br>- VIEW: Dimension Store [View (Dimension)] – not the local table<br>- VIEW: Time Dimension – Day [View (Dimension)] – not the local table

30. Ensure the Association for the Sales Manager table is based on the column ***Sales Manager ID*** in both tables. 
31. Ensure the Association for the Dimension Store View is based on the column ***Store ID*** in both tables. 
32. Ensure the Association for the time dimension is based on the columns ***Transaction Date*** and ***Date***.
 
33. In the Details panel now, click on the “More” option to navigate back to the main Properties window and
select the Fact option.
34. ***Deploy*** your View. (Deploying your view automatically saves your view)
35. You will be asked to confirm and ***Save*** the Business Name and Technical Name.

36. Once the view has been successfully deployed, you can now create your analytic model from the Model Properties screen.
<br>![](images/00_00_0888.png)

37. You should now be within your Analytic Model as depicted below. You're able to see the sales view and its associated dimensions that you added previously. 
<br>![](images/00_00_0889.png)

38. ***Deploy*** your Analytic Model.
39. Enter ***Sales - Analytic Model*** as Business Name and ***Save***. 

## Summary

You have now created and deployed your first Fact based View and Analytic Model. The Analytic Model can now be consumed within SAP Analytics Cloud.

Continue to - [Exercise 09: Business Layer - Dimension ](../ex09/README.md)
