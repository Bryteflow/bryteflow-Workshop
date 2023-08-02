---
title: "Connect source database connector" # MODIFY THIS TITLE
chapter: true
weight: 1 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Connect source database connector<!-- MODIFY THIS HEADING -->

## Connecting to MS SQL Server source database <!-- MODIFY THIS SUBHEADING -->
BryteFlow connects to any RDBMS sources using JDBC. 

Connect the SQL Server database as mentioned below:

1. In the Database Type select “Microsoft SQL Server Change Tracking” from the drop-down list.
2. In the Database Host field please enter the IP address or hostname of the database server
3. In the Database Port field please enter the port number on which the database server is listening on. The default port for MS SQL Server is 1433
4. In the Database Name field please enter the name of your database e.g. BryteMSSQL
5. Enter a valid MS SQL Server database user Id that will be used with BryteFlow Ingest. If a Windows user is required, please contact BryteFlow support info@bryteflow.com to understand how to configure this
6. Enter Password; then confirm it by re-entering in Confirm Password  
    - Please note, passwords are encrypted within BryteFlow Ingest
7. JDBC options are optional, can be used in order to extend the JDBC URL used to access the databases.
8. Click on the ‘Test Connection’ button to test connectivity
9. Click on the ‘Apply’ button to confirm and save the details


![Source database connection](/images/src1.png)
 
### Configure Destination database connector <!-- MODIFY THIS HEADING -->
Connect to Snowflake Data Warehouse as a destination connector for your pipeline. 
