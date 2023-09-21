# Exercise 14 - Best Salesperson

>:memo: **Note:** This is part of the <strong>Fast Track</strong> and a mandatory exercise.

---

In this exercise, we will we will setup a story in SAP Analytics Cloud based on our Consumption Layer, and review who
our best salesperson is.

1. Log On to your SAP Analytics Cloud tenant.
<br>![](images/00_00_0221.png) 
<br>

---

>:bulb: **Tip:** The system will ask you to resign in.

---

2. Select the menu Stories in the left-hand panel

3. Select the option Canvas to create a new Story.
<br>![](images/00_00_0201.png) 

4. Select "Optimized Design Experience" when asked "What design mode would you like to use?". Click "Create".
<br>![](images/00_00_0222.png) 

5. Under Widgets, select and drag the "Chart" onto the canvas.
<br>![](images/00_00_0204.png)
6. To select the model that you want to reference in your story<br><ul><li>select "DATASPHERE" as the connection on the left panel</li><li>select your SPACE e.g. ***GE12345***</li><li>For our third example, we will use the Perspective we created previously ***Revenue by Store and Product
(Perspective)***</li></ul>
<br>![](images/00_00_0206.png)

7. Now select the newly created empty chart on the canvas.
8. Navigate to the Builder Panel on the right hand side.
<br>![](images/00_00_0203.png) 

  
9. Click the option Add Dimension as part of the Dimensions section.
10. Select the option Create Dimension Input Control.
<br>![](images/00_00_0303.png) 
  
11. Select the entries:<br><ul><li>Dimension Store</li><li>Product</li><li>Sales Manager
<br>
  
12. Click OK.
<br>![](images/00_00_0307.png) 
  
13. On your canvas you will then be presented with a token for the newly created Dimension Input Control.
<br>![](images/00_00_0412.png) 

14. Select the token and resize the token so that you can see all entries.
<br>![](images/00_00_0413.png) 
  
15. Now use a double click on the header of the Dimension Input Control and enter: Please select a dimension.
16. Select the empty chart.
17. Navigate to the Business Builder Panel on the right hand side.
18. Click the Add Measure option for the Measures section.
19. Select measure Revenue.
<br>![](images/00_00_0210.png)  
  
20. Now open the More Actions menu for the chart.  
21. Select the menu Rank.  
22. Select the option Top N Options.
23. Set the Value to 10.
24. Click Apply. 
<br>![](images/00_00_0416.png) 
  
25. You should now have a chart showing the Top 10 entries based on the dimension selected with the input
control and based on the Consumption Layer created in SAP Datasphere.
<br>![](images/00_00_0417.png) 
  
25. In the File menu select the option to save your story.
26. Select the User folder that matches your assigned user number.
27. Enter a Name and Description like ***Best Salesperson***.
28. Click OK.  


## Summary

:trophy: Congratulations you have now completed the exercises for this session! 


