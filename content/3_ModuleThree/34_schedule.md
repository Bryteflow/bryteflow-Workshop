---
title: "Data Replication Schedule " # MODIFY THIS TITLE
chapter: true
weight: 4 # MODIFY THIS VALUE TO REFLECT THE ORDERING OF THE MODULES
---

# Scheduling <!-- MODIFY THIS HEADING -->
After the first initial sync is done, BryteFlow Ingest will continue with the incremental data replication at the specified schedule.

## Assign Data Replication Schedule<!-- MODIFY THIS SUBHEADING -->
 
BryteFlow replicates data in batches with a defined schedule as low as 1 second. 
To configure extracts to run at a specific time perform the following steps.

1. Go to 'Schedule' tab
2. For MS SQL Server you can choose the period in minutes.
3. A daily extraction can be done at a specific time of the day by choosing hour and minutes in the drop-down.
4. Extraction can also be scheduled on specific days of the week at a fixed time by checking the checkboxes next to the days and selecting hours and minutes in the drop-down.
5. Click on the ‘Apply’ button to save the schedule.
 
![Schedule tab](/images/sch.PNG)
