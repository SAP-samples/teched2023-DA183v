# Exercise 06 - Uploading Data

>:memo: **Note:** This is part of the <strong>Fast Track</strong> and a mandatory exercise.

---

In this exercise, we will populate the tables we have created in the previous steps, so that we have data for the analysis.

The files for this exercise are part of the ZIP file you downloaded in the beginning.
We will now upload the CSV files into the corresponding tables.
1. Log On to your SAP Datasphere tenant.
2. Select the menu option Data Builder on the left-hand side.
3. Use a double-click on the table Sales Transactions.
4. Select the menu option Upload Data from CSV File in the toolbar.
<br>![](images/00_00_0061.png) 

5. Click Choose ***File***.  
6. Navigate to where you unzipped the download.
7. Select the file ***“Sales Transactions.csv”***.
<br>![](images/00_00_0062.png) 

8. Ensure the option ***Delete Existing Data Before Upload*** is enabled.
9. Ensure the option ***Use first row as column header*** is enabled.
10. Ensure the option ***Insert missing string value as*** is set to ***NULL***.
11. Ensure the ***CSV Delimiter*** option is set to ***Auto-Detect***.
12. Ensure that all columns of the table have a mapped column from the CSV File.
13. Click ***Import***.
<br>![](images/00_00_0063.png) 

14. You should receive a message about the successful import of the information.
15. You can use the ***Data Preview*** to check if the data was loaded into the table.
<br>![](images/00_00_0206.png)

16. There is no need to save / deploy the table after you imported the data.

> :boom: ***Important*** :boom: <br> 
> 16. You can now continue and repeat the steps 4 - 15 for the other tables. Each table does have a corresponding CSV file as part of the download. Please upload the data for the following tables:<br>- Product (Dimension Product.csv)<br>- Store (Dimension Store.csv) <br>- Sales Manager (Dimension Sales Manager.csv)<br>


## Summary

Now you have imported all the data files and you can start to build the data model. 

Continue to - [Exercise 07: Creating the Dimension (part of <strong>Fast Track</strong> and a mandatory exercise)](../ex07/README.md)
