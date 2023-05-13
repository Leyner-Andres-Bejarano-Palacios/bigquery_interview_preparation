# bigquery_interview_preparation
:sunglasses: 

## Theorical Questions Section

### Theorical Question 1

Federated queries

<details><summary><b>Answer</b></summary>
Federated queries let you read data from external sources  (not stored in bigquery)
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/introduction
</details>

### Theorical Question 2

Do you know what On-demand compute (analysis) pricing

<details><summary><b>Answer</b></summary>
By default, queries are billed using the on-demand (per TB) pricing model, where you pay for the data scanned by your queries.

With on-demand pricing, you will generally have access to up to 2,000 concurrent slots, shared among all queries in a single project. Periodically, BigQuery will temporarily burst beyond this limit to accelerate smaller queries. In addition, you might occasionally have fewer slots available if there is a high amount of contention for on-demand capacity in a specific location.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/pricing#storage
</details>

### Theorical Question 3

Do you know what Capacity compute (analysis) pricing

<details><summary><b>Answer</b></summary>
Pricing for BigQuery editions is based on units of compute (slot hours) and offers pay as you go pricing (with autoscaling) and optional one year and three year commitments. 
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/pricing#storage
</details>

### Theorical Question 4

Do you know what is Flat-rate compute (analysis) pricing

<details><summary><b>Answer</b></summary>
When you enroll in capacity pricing, you purchase dedicated query processing capacity, measured in BigQuery slots. Your queries consume this capacity, and you are not billed for bytes processed. If your capacity demands exceed your committed capacity, BigQuery will queue up slots, and you will not be charged additional fees.  
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/pricing#storage
</details>

### Theorical Question 5

BI Engine pricing

<details><summary><b>Answer</b></summary>
BI Engine accelerates SQL queries by caching BigQuery data in memory. The amount of data stored is constrained by the amount of capacity you purchase. To purchase BI Engine capacity, create a BI Engine reservation in the project where queries will be run.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/pricing#storage
</details>

### Theorical Question 6

Do you know what table clone

<details><summary><b>Answer</b></summary>
Table clones are lightweight, writable copies of standard tables. BigQuery only stores the delta between a table clone and its base table.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>


### Theorical Question 7

Do you know what table snapshot

<details><summary><b>Answer</b></summary>
Table snapshots are point-in-time copies of tables. Table snapshots are read-only, but you can restore a table from a table snapshot. BigQuery only stores the delta between a table snapshot and its base table.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>


### Theorical Question 8

Do you know what Materialized views

<details><summary><b>Answer</b></summary>
Table snapshots are point-in-time copies of tables. Table snapshots are read-only, but you can restore a table from a table snapshot. BigQuery only stores the delta between a table snapshot and its base table.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>

### Theorical Question 9

What data type can you use as partition key

<details><summary><b>Answer</b></summary>
A time-unit column, such as a DATE or DATETIME column.

An integer column

The time when the data was ingested. In this case, BigQuery automatically stores the ingestion time in a pseudo-column that is not part of the table schema.
</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>


### Theorical Question 10

Clustering

<details><summary><b>Answer</b></summary>

![Image](img/clusteringBigQuery.png "clusteringBigQuery")

![Image](img/clusteringBigQuery_part2.png "clusteringBigQuery_part2")

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>

### Theorical Question 11

Intro Optimization

<details><summary><b>Answer</b></summary>

![Image](img/IntroQueryPlan.png "IntroQueryPlan")

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/storage_overview
</details>

### Theorical Question 12

Table Expiration day

<details><summary><b>Answer</b></summary>

![Image](img/tableExpiration.png "tableExpiration")

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/managing-tables#sql_1
</details>

### Theorical Question 13

Data lineage and whad tool to use

<details><summary><b>Answer</b></summary>

Data lineage is a Dataplex feature that lets you track how data moves through your systems: where it comes from, where it is passed to, and what transformations are applied to it. 

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/managing-tables#sql_1
</details>

### Theorical Question 14

Intro Cloud monitoring

<details><summary><b>Answer</b></summary>

![Image](img/cloudMonitoring.png "cloudMonitoring") 

![Image](img/introCloudMonitoringPerformance.png "introCloudMonitoringPerformance") 

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/monitoring/dashboards
</details>

### Theorical Question 15

Cloud Monitoring Samples

<details><summary><b>Answer</b></summary>

https://cloud.google.com/monitoring/docs/samples

https://cloud.google.com/docs/samples

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/monitoring/dashboards
</details>

### Theorical Question 16

Here you are monitoring how many products you are checking with cloud monitoringCloud Monitoring Samples

<details><summary><b>Answer</b></summary>

![Image](img/projectsByMonitoring.png "projectsByMonitoring") 

</details>

<details><summary><b>Source</b></summary>
https://www.youtube.com/watch?v=_FKdug6B5FM
</details>

### Theorical Question 17

Cloud logging

<details><summary><b>Answer</b></summary>

If you want to execute some action and see the result in real time there is a streaming log options that can show that streaming in the cloud logging service UI or in console using gcloud

![Image](img/cloudLogging.png "cloudLogging") 

</details>

<details><summary><b>Source</b></summary>
https://www.youtube.com/watch?v=IlUCyV8mcS0
</details>




### Theorical Question 18

In biquery datasets what does it mean logical and phisical billing

<details><summary><b>Answer</b></summary>

If you want to execute some action and see the result in real time there is a streaming log options that can show that streaming in the cloud logging service UI or in console using gcloud

![Image](img/phisycalLogicalBillingBiquery.png "phisycalLogicalBillingBiquery") 

![Image](img/physicalLogicalBigquery_part2.png "physicalLogicalBigquery_part2") 

</details>

<details><summary><b>Source</b></summary>
https://cloud.google.com/bigquery/docs/datasets
</details>
