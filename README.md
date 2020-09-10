# QuickTableViewer Extension
Qlik Sense Extension to quickly get all fields of a data-model table into a standard Qlik Sense Table object.

**New 10-Sep-2020**: a checkbox that allows to remove a (table-)prefix from Field Names in the label of the column e.g. Customers.Name -> Name 
(everything before the first "." is removed then)

* Place the extension on the sheet where you like to get the table object
* select from the properties panel on your right which table you would like to see
* you can specify a pattern for both, fields to include (default: *) and fields to exclude (default: %* ... all fields starting with %)
* after you click the button "Get My Table" the object manipulates itself to become a standard Sense table object

Authors: 
 - Christof Schwarz, formerly Qlik, now data/\bridge
 - [Ralf Becher](https://github.com/ralfbecher), formerly TIQ Solutions, now Vizlib

Thanks to Ralf, you can select multiple tables at once to get columns from more than 1 table. The code checks if there is a connection in the data model between the tables before adding its columns to avoid cartesean products with out-of-memory results. Ralf explains this here --> https://medium.com/@irregularbi/do-my-tables-associate-dc249d59ee89

![alt text](https://github.com/ChristofSchwarz/pics/raw/master/quicktableview.gif "Screenshot")
