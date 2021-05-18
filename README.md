# SSRS-Report
SSRS Report With Grouping of Data having hide and unhide feature in excel of grouped data


# Requirements 
## Your system must have the following components installed:

1. Microsoft SQL Server database engine.
2. SQL Server 2016 Reporting Services or later (SSRS).
3. The AdventureWorks2016 database. 
https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2016.bak
4. SQL Server Data Tools for Visual Studio along with the Reporting Services extension installed to enable access to the Report Designer.

# create a report server project

1. From the File menu, select New > Project.
2. In the left-most column under Installed, select Reporting Services. In some cases, it may be under the group Business Intelligence.
3. Select the Report Server Project icon in the center column of the New Project dialog box.

# Creating a report definition file (RDL)

1. In the Solution Explorer pane, right-click on the Reports folder. If you don't see the Solution Explorer pane, select View menu > Solution Explorer.
2. In the Add New Item window, select the Report icon.
3. Type "Sales Orders.rdl" into the Name text box. Select the Add button on the lower right side of the Add New Item dialog box to complete the process.
   Report Designer opens and displays the Sales Orders report file in Design view.
   
# To set up a connection

1. In the Report Data pane, select New > Data Source. If the Report Data pane isn't visible, then select View menu > Report Data.
2. In the Name text box, type "AdventureWorks2016".
3. In the Connection string text box, type the following string:
      Data source=localhost; initial catalog=AdventureWorks2016
4. Select the Credentials tab, and under the section Change the credentials used to connect to the data source, 
   select the Use Windows Authentication (integrated security) radio button. Select OK to complete the process      

# Define a Transact-SQL query for report data

1. In the Report Data pane, select New > Dataset.... The Dataset Properties dialog box opens with the Query section displayed.
2. In the Name text box, type "AdventureWorksDataset".
3. From the Data source dropdown box, select AdventureWorks2016.
4. For the Query type, select the Text radio button.
5. Type Transact-SQL query into the Query text box.

# Preview Reportin Visual Studio and download

Select the Preview tab. Report Designer runs the report and displays it in the Preview view. 


