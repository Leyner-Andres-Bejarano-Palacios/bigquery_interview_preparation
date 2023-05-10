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

