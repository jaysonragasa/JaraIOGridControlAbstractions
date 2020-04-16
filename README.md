# FORKED
forked from my old GitHub account Nullstr1ng

# JaraIOGridControlAbstractions
Create an inline Row and Column defenitions for Grid control in Xamarin

![](https://pbs.twimg.com/media/EU93F1sU8AImkUg?format=png&name=large)

# History
## 1.2
* Added two new attached attributes called GridDefinitions and RowColumns
* You can use tilde (~) as an alternative to Auto
* Space as an alternative to comma (,)
* Slash (/) to separate Rows and Columns

i.e  
**GridDefinitions="~ \* / \* \*"**  
-- This will create 2 rows and 2 columns. The height of the first Row is set to Auto and the second is set to Star. Two new columns are set to Star. Note: Doesn't matter if you added spaces before and after the Slash. So it can be ="~ \*/\* \*"  
**GridDefinitions="~ ~/\*2 \*"**  
-- This is another example  
**GridDefinitions="/\*2 \*"**  
-- Notice the slash as the first chracter. This will create a column instead of a row.  
**GridDefinitions="\*2 \*/"**  or **GridDefinitions="\*2 \*"**  
-- Notice the slash at the end or the other doesn't have it? This will create rows only!  
**GridDefinitions="Auto ~ \*,\*"**  
-- This will create four rows. First and second row is set to Auto. Third and Forth are set to Star  
**RowColumn="0/1"**  
-- Will set the current element in the first row of the grid and in second column of the grid.  
**RowColumn="0 2/1"**  
-- Will set the current element in the first row of the grid spanning upto the second and then it will place the element in the second column.

## 1.1
* Added support for Absolute values. Originally accepting Auto * and n# only. So you can use Auto * n* and n now.  
i.e RowDefinitions="Auto,\*,3*,50"

## 1.0
* Implementation of RowDefinitions and ColumnDefinitions attached attributes
