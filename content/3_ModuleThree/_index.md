---
title: "Data Replication Pipeline Setup" # MODIFY THIS TITLE IF APPLICABLE
chapter: true
weight: 3
---

# Data Replication Pipeline Setup <!-- MODIFY THIS HEADING -->

## Configure your own data replication pipeline <!-- MODIFY THIS SUBHEADING -->

In this workshop we are going to showcase the SQL Server to Snowflake usecase of BryteFlow. The pipeline has to be setup to replicate data from a MS SQL Server Database to Snowflake.

Setting pipeline with BryteFlow in 3 easy steps:  
1. Connect source database
2. Connect destination database
3. Select tables and start replicating

#### Connect source database connector<!-- MODIFY THIS SUBHEADING IF APPLICABLE -->
Connect to MS SQL Server DB in quick and easy steps.

{{% notice warning %}}
The examples and sample code provided in this workshop are intended to be consumed as instructional content. These will help you understand how various AWS services can be architected to build a solution while demonstrating best practices along the way. These examples are not intended for use in production environments.
{{% /notice %}}

### Configure Destination database connector <!-- MODIFY THIS HEADING -->
Connect to Snowflake Data Warehouse as a destination connector for your pipeline. 