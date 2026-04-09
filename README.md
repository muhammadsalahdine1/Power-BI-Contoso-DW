# Power-BI-Contoso-DW
## Dataset Contoso-data 
FactStrategyPlan - DimAccount - DimDate - DimEntity - DimProductCategory - DimProductCategory
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/c.PNG" width="1000">

## Let's breakdown the report by questions?

### Changing visuals
### Time to get to work! I'm are going to change and format visuals. 
### First, I'll turn the donut chart into a tree map to get a better understanding of the product categories. 
### Then, I'll change the simple card visual to a multi-row card by adding scenario name to it so that it's possible to closely track the actual, forecasted, and budgeted amounts.
<div>
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/a.PNG" width="500">
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/b.PNG" width="500">
<\div>

### I want to see the data in a summarized way so the table needs to become a matrix.
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/d.PNG" width="1000">

### Sorting is a common method used for visualizing data in a form that makes it easier to comprehend the story the data is telling. 
### Sort the months in the bar chart in the correct order, from January to December. This will make it easier to interpret the visual and look at amount changes over time.
- Go to the Data View to make sure that ShortMonth in the DimDate table is ordered by MonthNumber.
- Go back to the report and sort the columns in the Monthly Amount visual by month instead of amount.
- Sort the months in ascending order.
- How is the sales amount evolving throughout the year?
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/e.PNG" width="1000">

### Let's apply some more advanced formatting to our report. You find that the slicer in the top right takes up a bit too much space in the report. 
#### There are a lot of categories and it would be better to not show them all but enable users to select from a dropdown menu instead.
- Go to the formatting options and turn off the slicer header.
- Change the slicer to a dropdown box
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/f.PNG" width="1000">

###  it's worth taking a final pass and making sure everything is looking great.
### I'll format the report by changing the background color and making sure every visual has an appropriate size. 
- Change the theme of the report to the Sunset theme.
- Adjust the height of the dropdown box to be the same as the multi-row card.
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/g.PNG" width="1000">

### Looking at the data
### If you'd like to see the data that Power BI uses to create a visualization, you can display that data. You can even export the data as an .xlsx or .csv file so you can open it in Excel later.Here, I'll look at the data and export it to a csv file that I will then open up with Windows' default text editor, Notepad.
- Select the clustered column chart.
- Display the underlying data.
- Export the data as a .csv file and save it on the desktop.
- Save the file as MonthlyAmount.csv and take a look at the file.
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/h.PNG" width="1000">

### Creating a hierarchy
#### Sometimes you want to drill down into a chart and see different levels of your data. With hierarchies, you can add this functionality to your Power BI reports. Let's create a date hierarchy that looks like this: Year-Quarter-Month-Day.
- Navigate to the DimDate table in the Table view.
- Create a hierarchy that starts with Year, goes on to the QuarterFull, then the MonthName, and ends with the DateKey.
- You can create a hierarchy by dragging QuarterFull on top of Year.
- Do the same for MonthName and DateKey.
- Or select "Create hierarchy". From there, you can right-click the necessary fields and select "Add to hierarchy".
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/i.PNG" width="1000">

 ### In the column chart on the Report view, replace the ShortMonth Axis value of the column chart by the Date Hierarchy.
 - Use the drill controls in the top right corner of the visual to explore the different levels.
 - Which quarter across all years had the highest amount ?\
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/j.PNG" width="1000">

### Adding a filter
#### Filtering is an important tool when you're creating Power BI reports. You don't always want to look at all of the data. Limiting the data used in visuals to only a selection that is relevant can help you answer more detailed business questions.
- In the report, I can see that the cards on the Sales Analysis page tab are labeled Actual, Forecast, and Budget, but they all have the same values. 
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/k.PNG" width="1000">

- I'll need to apply some filters to fix this.
- Open the Filters pane.
- Add a filter to the "Actual" card visual that filters on rows where ScenarioName is equal to Actual.
- Select the visual.
- Drag the field ScenarioName of the DimScenario table to the Filters on this visual section.
- Click on the required check box.
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/l.PNG" width="1000">

- Add a filter to the "Forecast" card visual that filters on rows where ScenarioName is equal to Forecast.
- Add a filter to the "Budget" card visual that filters on rows where ScenarioName is equal to Budget.
- Question: What was the total forecasted amount?
<img src="https://github.com/muhammadsalahdine1/Power-BI-Contoso-DW/blob/main/m.PNG" width="1000">
 

 


