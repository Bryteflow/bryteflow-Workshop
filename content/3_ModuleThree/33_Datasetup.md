---
title: "Choose data to be replicated " # MODIFY THIS TITLE
chapter: true
weight: 3 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Choose data to be replicated <!-- MODIFY THIS HEADING -->
Once connected to the source database, select all objects or objects of your choice to be added to the replication pipeline.

##Select tables for replication <!-- MODIFY THIS SUBHEADING -->
BryteFlow list all tables from SQL Server, from accross databases and schema in the data catalogue for users to select tables and start replication.

Please make sure to perform the source database prerequisites for the table of interest.
For prerequisite steps please refer to User guide : https://docs.bryteflow.com/bryteflow-setup-guide#using-sql-server-change-tracking

Once done select the table for transferring to destination database, perform the following steps.

1. In the 'Data' tab expand the Database.
2. Browse to the table you want to be synced with Amazon Redshift or Amazon S3.
3. Select the checkbox next to the table and then click on the table.
4. On the right-hand side pane, select the type of transfer for the table i.e. By Primary Key or By Primary Key with History. With the Primary Key option, the table is replicated like for like to the destination. With the Primary Key with History option, the table is replicated as time series data with very change recorded with Slowly Changing Dimension type2 history (aka point in time)
5. You can also mask a column by checking the checkbox. By masking a column, the selected column will not be transferred to the destination.
6. Click on the ‘Apply’ button to confirm and save the details
7. This process of selecting tables, configuring primary keys and mask columns should be repeated for each of the tables. Once complete the next step is to:
8. Navigate to the Schedule tab
9. Click on the ‘Full Extract’ button to initiate the Initial Extract and Load process

This will initiate the very first initial data sync from SQL Server to Snowflake and thereafter continue with the incremental data replication as per the schedule.
