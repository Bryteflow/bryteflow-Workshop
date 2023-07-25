---
title: "Partner Setup" # MODIFY THIS TITLE IF APPLICABLE
chapter: true
weight: 3
---

# Partner Setup <!-- MODIFY THIS HEADING -->

## Configure your own data replication pipeline <!-- MODIFY THIS SUBHEADING -->

In this workshop we are going to showcase the SQL Server to Snowflake usecase of BryteFlow. The pipeline has to be setup to replicate data from a MS SQL Server Database to Snowflake.

Setting pipeline with BryteFlow in 3 easy steps:  
1. Connect source database
2. Connect destination database
3. Select tables and start replicating

#### Connect source database connector<!-- MODIFY THIS SUBHEADING IF APPLICABLE -->
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

{{% notice warning %}}
The examples and sample code provided in this workshop are intended to be consumed as instructional content. These will help you understand how various AWS services can be architected to build a solution while demonstrating best practices along the way. These examples are not intended for use in production environments.
{{% /notice %}}

### Configure Destination database connector <!-- MODIFY THIS HEADING -->
Connect to Snowflake Data Warehouse as a destination connector for your pipeline. 