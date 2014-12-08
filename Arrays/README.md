Example Velocity Scripts for Cascade Server
============================================

The following scripts demonstrate the usage of Arrays and Dictionaries/Associative Array in Velocity. 

Description of the scripts:

* ArchiveMonthLocatorTool.vm: We use this script to archive news articles of each month. Associative Arrays are highly resourceful here, since it allows us to store information about all articles(name, link, teaser, date), associated with their categories(which are the keys), in just one comprehensive data structure, and then allows us to manipulate or access these in any way needed.

* DatesDisplay.vm: We use this script to display dates on our admissions page. This script shows the use of plain, one-dimensional arrays. The arrays are used to store the names and links of all the events, extracted from the calendar, which allows us to check for consecutive events, by iterating through the arrays and then displaying them in a more elegant "StartDate - EndDate: EventName" format.

* LayoutsTable.vm: We use this script for internal surveys about the number of pages using each layout type. This script also demonstrates using associative arrays, with arrays as values. Similar to ArchiveMonthLocatorTool, the associative array lets us store information about the pages. and then access and display them while drawing the table.


**NOTE about Iteration through Arrays:**

In Velocity, syntax for iteration would be:

```
#for ($element in $array)
	## Body
	## Operations on $element
#end
```
This is similar to the iteration in Python.


