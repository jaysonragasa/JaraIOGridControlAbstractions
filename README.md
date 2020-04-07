# JaraIOGridControlAbstractions
Create an inline Row and Column defenitions for Grid control in Xamarin

# History
## 1.2
* Added two new attached attributes called GridDefinitions and RowColumns
* You can use tilde (~) as an alternative to Auto
* Space as an alternative to comma (,)
* Slash (/) to separate Rows and Columns

i.e  
**GridDefinitions="~ \* / \* \*"**  
-- This will create 2 rows and 2 columns. The height of the first Row is set to Auto and the second is set to Star. Two new columns are set to Star. Note: Doesn't matter if you added spaces before and after the Slash. So it can be ="~ \*/\* \*"  
**RowColumn="0/1"**  
-- Will set the current element in the first row of the grid and in second row of the grid.  
**RowColumn="0 2/1"**  
-- Will set the current element in the first row of the grid spanning upto the second and then it will place the element in the second column.

## 1.1
* Added support for Absolute values. Originally accepting Auto * and n# only. So you can use Auto * n* and n now.  
i.e RowDefinitions="Auto,\*,3*,50"

## 1.0
* Implementation of RowDefinitions and ColumnDefinitions attached attributes
