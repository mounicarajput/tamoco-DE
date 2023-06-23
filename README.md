
Note: If the problem occurs rendering the ```ce.ipynb``` file then you can use https://nbviewer.org/ to  view the Jupyter notebook.
We just need to add the notebook URL : https://github.com/mounicarajput/tamoco-DE/blob/main/ce.ipynb

# Technical Questions

Open ```dataeng.txt``` file to view detailed explanation of the below Questions.

## Q1 - Spark

Tamoco uses Spark for most of the ETL workloads. When saving the final data, we have an ideal target file size of around 115MB. Explain how you would make sure that output files are approximately this size.


## Q2 - CI/CD

Tamoco uses Apache Airflow for orchestration. Airflow code is stored in a Github repository, and we have a simple CI/CD pipeline built with AWS CodeBuild that copies any code merged into the main branch of this repository into an S3 bucket. Describe how you would add a step that checks that validates all the Airflow DAGs before merging into the main branch.


## Q3 - AWS Services

Tamoco regularly needs to send large amounts of data to clients (in the TBs range). Assuming you know the exact location of the files inside Tamoco’s S3 bucket, describe how you would send a large amount of data to an external S3 bucket. In addition, outline how you would estimate the overall cost of the transfer.


## Coding Exercise
Open ```ce.ipynb``` Notebook to see the below analysis.

- Remove the unnecessary columns and duplicated pings in the data set.

- Find the location and time range of data.

- Calculate the average number of pings per device.

- Plot the distribution of accuracy of Android devices.

- Find the hour in which devices sent the most pings.

- Find the number of redundant pings in the data set. If a device sends more than 2 pings with a rate greater than 1 ping/hour from the same location (the same latitude/longitude), pings except the first and last ones are redundant.





