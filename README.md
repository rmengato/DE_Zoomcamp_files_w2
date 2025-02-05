# DE_Zoomcamp_files_w2

Files used for answering Data Engineering Zoomcamp, module 2.

The yaml file is meant to be interpreted by Kestra, the orchestrator of choice for this week's module.
Not much is changed from William's code, apart from name changing in a KV pair.
Questions could be answered through the use of Backfill functionality.
Unfortunatelly, the challenge of iterating through combinations by using the forEach functionality is not currently present. It may be implemented in coming weeks or be used first within the final project.



Answers were reached, when applicable, through SQL queries in BigQuery, such as the query performed below:

SELECT COUNT(1)
FROM `de-zoomcamp-rmengato.zoomcamp.yellow_tripdata`
WHERE TIMESTAMP_TRUNC(tpep_pickup_datetime, YEAR) = TIMESTAMP('2020-01-01');

In other cases, answers could as well be reached through reading of Kestra's documentation, for instance in the case of the timezone.
