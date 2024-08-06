# DQThon ETL Project
participants data for the hackathon organized by DQLab named DQThon

## Overview
This project demonstrates an ETL (Extract, Transform, Load) pipeline for processing and transforming a dataset of DQThon participants using Apache Spark and SQL. The dataset is sourced from a S3 Bucket, and the transformed data is loaded into a SQL database. This project highlights the use of Apache Spark for efficient data processing and SQL for structured data storage and querying.

## Project Structure
- **Extract**: Load the participant data from an S3 Bucket into a Spark DataFrame.
- **Transform**: Perform various data transformation steps, including:
  - Extracting postal codes and cities from the address field.
  - Generating GitHub profiles and cleaned phone numbers.
  - Creating team names and emails based on participant details.
  - Formatting birth dates and registration times.
- **Load**: Write the transformed data into a SQL database using JDBC.

## Technologies Used
- **Apache Spark**: For distributed data processing and transformations.
- **SQL**: For structured data storage and querying.

## Dataset
The dataset consists of participant information for a DQThon event, including fields such as first name, last name, address, phone number, birth date, registration time, country, and institute. The dataset is provided in Amazon S3 Bucket located at **`s3://dqthon-hackathon-data/dqthon-participants.csv`**.
