# Exercise 12 - Top 10 Revenue Generating Products

> :memo: **Note:** This is part of the <strong>Fast Track</strong> and a mandatory exercise.

---

In this exercise, we will setup a story in SAP Analytics Cloud, which allows us to view the Top 10 Revenue Generating Products.

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
6. To select the model that you want to reference in your story<br><ul><li>select "DATASPHERE" as the connection on the left panel</li><li>select your SPACE e.g. ***GE12345***</li><li>for our first example, select your ***Sales - Analytic Model***</li></ul>
<br>![](images/00_00_0205.png)

7. Now select the newly created empty chart on the canvas.
8. Navigate to the Builder Panel on the right hand side.
<br>![](images/00_00_0203.png) 


9. Click Add Dimension as part of the Dimensions section.
<br>![](images/00_00_0209.png) 

10. Select Transaction Date & Product ID.
<br>![](images/00_00_0202.png)
>:bulb: Ensure the Transaction Date is positioned first within the Dimensions section.  

11. Click Add Measure as part of the Measures section.
12. Select measure Revenue.
<br>![](images/00_00_0210.png)

13. Click on the Filter icon for dimension Transaction Date.
14. Select the option Filter by Member.
<br>![](images/00_00_0215.png) 
15. Open the list of members and select the year 2022.
16. Click OK
<br>![](images/00_00_0216_2.png)
17. Open the More menu (...) for the chart (top right corner of chart).
18. Within the menu, go to Rank > Top N Options > Update value to "10".
19. Click Apply.
<br>![](images/00_00_0220.png)

20. Update Chart Orientation to ***Horizontal*** in the Builder Panel.
21. You can adjust the sizing of the chart by clicking and dragging the brackets outward or inward.
<br>![](images/00_00_0223.png)

22. Your chart should look like this.
<br>![](images/00_00_0225.png) 

23. In the File menu select the option "save" to save your story.
24. Create a User folder that matches your Space name,  e.g. ***GE12345***.
<br>![](images/00_00_0224.png) 
25. Enter a Name and Description like ***Top 10 Revenue Generating Products***.
26. Click OK.

## Summary

You've now created your first SAP Anayltics Cloud Story on top of the data model you created earlier. 

Continue to - [Exercise 13: Revenue by Geography (requires Exercise 08 to be completed) ](../ex13/README.md)
