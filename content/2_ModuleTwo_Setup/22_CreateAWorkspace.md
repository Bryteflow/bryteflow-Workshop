---
title: "Create a Workspace" # MODIFY THIS TITLE
chapter: true
weight: 2 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

 <!-- MORE SUBMODULES CAN BE ADDED TO DIVIDE UP THE SETUP INTO SMALLER SECTIONS -->
<!-- COPY AND PASTE THIS SUBMODULE FILE, RENAME, AND CHANGE THE CONTENTS AS NECESSARY -->


# Set Up The Workspace <!-- MODIFY THIS SUBHEADING -->

## Set Up Your Workspace <!-- MODIFY THIS SUBHEADING -->
 BryteFlow allows real-time Data Replication & Integration for Amazon S3, Amazon Redshift and Snowflake Data Warehouse.  
 
## Highlights <!-- MODIFY THIS SUBHEADING -->  
- Data Ingestion: Automated Real-time integration to S3, Redshift and Snowflake using Change Data Capture (CDC) technology, with zero load on the source.  
- Data Preparation: Reduce Data deployment from months to hours. Automated high performance time series data build, data ingested real-time, prepared and ready to use. Transform and prepare your data assets with a self serve intuitive GUI  
- Data Reconciliation, High Availability, resiliency and scaling with terabytes of data is built into the software.

We will launch BryteFlow Standard Edition from AWS Marketplace from the AWS account. There are a few steps to complete to set this up:  
  
  - Launch BryteFlow from AWS Marketplace
  - Create an IAM role for your workspace
  - Attach the IAM role to your workspace
  - Configure workshop specific requirements


 
### Launch BryteFlow Standard Edition <!-- MODIFY THIS HEADING -->

BryteFlow is the replication Software for Easy Enterprise Data Integration
It is a no-code data replication software that replicates your data using CDC from transactional sources like SAP, Oracle, SQL Server, MySQL and PostgreSQL to popular platforms like AWS, Azure, SQL Server, BigQuery, PostgreSQL,  Snowflake, Teradata, Databricks and Kafka in real-time, providing ready to use data on the destination. Our data replication software is automated, GUI driven, self-service and offers out-of- the-box support for bulk data.

### Launch BryteFlow Ingest from AWS Marketplace : Standard Edition <!-- MODIFY THIS SUBHEADING -->

Steps to launch BryteFlow Ingest from AWS Marketplace: Standard Edition 

1. Please ensure to complete the ‘Environment Preparation‘ section before proceeding to launch BryteFlow from an AMI.

2. Go to the product URL https://aws.amazon.com/marketplace/pp/B01MRLEJTK

3. Click ‘Continue to Subscribe’ 

4. Click ‘Continue to Configuration’. This brings up the default ‘Fulfillment Option’ with the latest software version.

5. Choose the AWS Region you would like to go for or else go by the default AWS Region that is already present in the dropdown.
6. Click ‘Continue to Launch’
7. Choose Action ‘Launch from Website’
8. Select your EC2 instance type based on your data volume, recommendations available in the product detail page
9. Choose your VPC from the dropdown
10. Please select the ‘Private Subnet’ under ‘Subnet Settings’. If none exists, its recommended to create one. 11. Please follow detail AWS User Guide for Creating a Subnet.
12. Update the ‘Security Group Settings’ or create one based on BryteFlow recommended steps as below:
13. Assign a name for the security group, for eg: BryteFlowIngest
14. Enter a description of your choice
15. Add inbound rule(s) to RDP the EC2 with the Custom IP address
16. Add outbound rule(s) to allow the EC2 instance access the source db. DB ports will vary based on the source database , please add rules to allow the instance access to specific source database ports.
        For more details, refer to BryteFlow recommendation on Network ACLs for your VPC in the below section ‘Recommended Network ACL Rules‘
17. Provide the Key Pair Settings by choosing an EC2 key pair of your own or ‘Create a key pair in EC2‘
18. Click ‘Launch’ to launch the EC2 instance.
19. The endpoint will be an EC2 instance running BryteFlow Ingest (as a windows service) on port 8081


Info: This will take about 1-2 minutes to provision
