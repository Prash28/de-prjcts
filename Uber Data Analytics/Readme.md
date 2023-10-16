Uber Data Analytics project on Google Cloud Platform(GCP):

	1. First Uber dataset is loaded onto Google cloud storage(GCS) bucket.
	2. Then, a Dimensional model was built and the data was loaded into BigQuey after performing transformations.
	3. Finally, a Looker Dashboard was built for analysis.

This process is orchestrated by Mage, a modern ETL tool.

# Uber Data Analytics - Data Engineering GCP Project

## Introduction

The goal of this project is to perform data analytics on Uber data through tech and tools namely GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

## Architecture 
![](https://drive.google.com/uc?export=view&id=1tGbbw0fnLCmySMeyd79_qDbueTvmtzT- "snap_1")

## Technology Used
- Programming Language - Python

Google Cloud Platform
1. Google Storage
2. Compute Instance 
3. BigQuery
4. Looker Studio

Modern Data Pipeine Tool - https://www.mage.ai/

## Dataset Used
TLC Trip Record Data
Yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts. 

More info about dataset can be found here:
1. Website - https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
2. Data Dictionary - https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

## Data Model
![](https://drive.google.com/uc?export=view&id=1ARNx7iEjTP4uijTjIrVajRakKDMM-ps8)

Link to the original Project idea by Darshil Parmar: https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project

**Project Workflow:**

1. Extracting data from TLC Trip Record Data website:

![](https://drive.google.com/uc?export=view&id=1A1QC-CRuFe5DLfaAn1501gFgvrDL_UUL)

2. Storing the csv file in GCS Bucket:

![](https://drive.google.com/uc?export=view&id=1NK6ibSFKXWae6BRJVCDZGNm3xkneJisA)

3. Creating VM Instance in Google Compute Engine:

![](https://drive.google.com/uc?export=view&id=1R8aTefc-DVrO73IKUimukhY9zyi3fB87)

4. Orchestating the project using Mage:
   Ran Mage in the GCP VM Instance.

![](https://drive.google.com/uc?export=view&id=1JWwSD2IOlGf7uDGIfm8gnDvGqPpdntpV)

Performed ETL Operation and loaded the fact and dimensional tables to BigQuery.

![](https://drive.google.com/uc?export=view&id=17p7aX43KoEumDGUycbvxbnu_GzAa6q8f)

5. Created tbl_analysis by joining the fact and dimensional tables for our analysis.

![](https://drive.google.com/uc?export=view&id=1Md7os7MlrzXuY2Jyhh3fnFDugB-iLsuR)

6. Imported the tbl_analysis table into Looker Studio and created dashboard with filters to work with.

![](https://drive.google.com/uc?export=view&id=1bKn4-rPj-raTK5kaZ_x8Y6CA8l8O-ywn)

See the full Looker Studio report here: https://drive.google.com/file/d/1RijAJwWsVoke04IHqllryrKIGhAM-x2U/view?usp=drive_link
 
