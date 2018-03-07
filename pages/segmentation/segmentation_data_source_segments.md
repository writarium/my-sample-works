---
title: "Data Source Segments"
keywords: segmentation, building, data, data source segments, data, source, segments
sidebar: seg_building_sidebar
permalink: segmentation_data_source_segments.html
summary: "As you build segments using the point-and-click method of Teradata RM, you may want to  enter your own SQL queries or modify the existing ones."
folder: segmentation
---

## Defining data source segments
### Data Source Types
The point-and-click method of defining segments is the most commonly used method in Teradata RM. However, there may be instances when this method does not provide you the desired results. To overcome this situation, Teradata RM provides alternatives for defining segments. In the next subsections, we take a look at these alternatives.

### Working with User-Defined Views (UDV)
In this method of defining segments, you can use SQL to obtain leads. The SQL specifies the columns to be obtained from the data warehouse tables. There are two ways to create a UDV. First, you select CRM > Segmentation > User-define Views option from Applications menu. The next figure illustrates this selection:

<img src="images/AdvSegBuilding.jpg">

Alternately, click the drop-down list next to Workspace and choose UDV. In either ways, the screen to create a UDV appear as illustrated in the next figure.

<a data-fancybox="gallery" href="images/UDV-Definition-Editor.jpg" title="click to enlarge" alt="UDV definition editor">
<img src="images/UDV-Definition-Editor.jpg" style="width: 400px;"/>
</a>


The next procedure describes the steps to create a UDV.
### Creating a User-Defined View (UDV)
1. In UDV Name, enter the name for the UDV.
2. In Description, enter a description.
3. In Locking SQL, enter your query for locking the tables required in Base SQL.
4. In Base SQL, enter your query for the UDV. The SQL drives selection of attributes from tables appearing in the SQL.
5. Click Populate from SQL to drive the columns in the Column names table. This table is populated only if the SQL entered in Base SQL is valid.
6. Give alternate names in Column names table that best explain the data contained in them.
7. Click Validate to ensure that the UDV details you have entered are valid and can lead to successful selection.
8. Click Save to select your UDV.
9. If you want to make a copy of your UDV, select Save As and give a new name to the UDV.


### Working with warehouse tables and acquisition lists
In this method of defining segments, you can use a warehouse table whose columns have not been mapped through metadata. A warehouse table is generally used along with an acquisition list. An acquisition list is any formatted data file that is obtained from some external source. Typically, an acquisition list contains customer data of an external enterprise that can become a source of lead for your business. 

After defining a warehouse table, you populate the table by importing data from an acquisition list. You can create a warehouse table using Warehouse Table Definition screen. There are two ways to invoke the Warehouse Table Definition screen. You either click Warehouse Tables in Applications menu or the drop-down list next to Workspace and choose Warehouse Table. In either ways, Warehouse Table Definition screen appears as illustrated in the next figure.

<a data-fancybox="gallery" href="images/Warehouse-Table-Definition.jpg" title="click to enlarge" alt="Warehouse Table Definition">
<img src="images/Warehouse-Table-Definition.jpg" style="width: 400px;"/>
</a>

### Creating a warehouse table definition:
1. In Name, enter the name for the warehouse table definition.
2. In Description, enter a description.
3. In Database, select the database that stores the warehouse table definition.
4. In Table, select the table name.
5. Click Populate from Table to locate columns from the selected table, and place them in the table beneath Populate from Table.
6. Click to add or to delete columns from the list box. You can also enter a column expression, such as Col1+Col2, in the new column.
7. Click Import to display the Import dialog containing options for importing data from an external file.
8. Click Save As to save the warehouse table definition that can be used later, as a source of leads for a segment.
{% include links.html %}
