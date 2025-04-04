
# End to End Project on Data Engineering

<p style="text-align: justify;">
This project is demostration which involves data ingestion, raw data transformation and finally transformed data is used for data analysis to provide valuable insights using Microsoft Azure cloud platform.
</p>

![Flow chart](https://github.com/Sathyam-Kakodkar/Azure-Data-Engineering-Project/blob/main/images/flow%20chart.png)


## Data Source

The data contains multiple files in the csv format. It is stored in the GitHub repository.

Dataset --> [Data Source.csv](https://github.com/Sathyam-Kakodkar/Azure-Data-Engineering-Project/tree/main/data)

## Azure Data Factory 


![ADF](https://github.com/Sathyam-Kakodkar/Azure-Data-Engineering-Project/blob/main/images/data%20factory.png)

This is used for data ingestion. So firstly, data pipeline is created. Here we have given the path to the source and sink. Source is the GitHub repository were all the files are present and sink is the raw storage folder in the Data Lake Gen 2. Follow the same procedure for the connecting the remaining data files.


## Azure Databricks

![Databricks](https://github.com/Sathyam-Kakodkar/Azure-Data-Engineering-Project/blob/main/images/databricks.png)

Create new workspace, create compute, and then open new notebook. We must make use of the Py Spark code for reading the files from raw storage of data lake gen 2 and then transform the files and write it into the transformed storage directory in the data lake.

## Azure Synapse Analytics

![Synapse](https://github.com/Sathyam-Kakodkar/Azure-Data-Engineering-Project/blob/main/images/synapse.png)

<p style="text-align: justify;">
Create new synapse workspace and select lake database and write the path to the transformed data stored in data lake. Perform necessary analytics on stored tables as per requirement. Further you can connect this database to power bi or any other bi tool to create visualization and dashboards.
</p>