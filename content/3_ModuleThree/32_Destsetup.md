---
title: "Connect destination database connector" # MODIFY THIS TITLE
chapter: true
weight: 3 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Connect destinaton database connector<!-- MODIFY THIS HEADING -->

## Connecting to Snowflake Data Warehouse <!-- MODIFY THIS SUBHEADING -->
BryteFlow connects to Snowflake using JDBC. 

Connect to Snowflake data warehouse as mentioned below:

1. Go to Destination Database
2. Enter ‘Database Type’ as ‘Load to Snowflake direct’
3. Database host is the Snowflake account URL For eg: abc123.ap-southeast-2.snowflakecomputing.com
4. Provide Snowflake Account name under ‘Account name’
5. Enter Snowflake Data warehouse name in ‘Warehouse Name’ field
6. Enter Snowflake Database name in ‘Database Name’ field
7. Enter Snowflake UserID in the Userid field
8. Password to be configured under Password and Confirm Password section.
9. JDBC options are optional, in order to extend the JDBC URL used to access the databases.
10. Click on the ‘Test Connection’ button to test the connection details
11. Click on the ‘Apply’ button to confirm and save the details


![Destination database connection](/images/SFLKs3.png)
 
 
### Choose data to be replicated <!-- MODIFY THIS HEADING -->
Once connected to the source database, select all objects or objects of your choice to be added to the replication pipeline.
