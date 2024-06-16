# BritCovid_DataStream

## Overview
BritCovid_DataStream is a data engineering project designed to ingest, process, and analyze COVID-19 data in the UK. The project leverages various Azure services, including Azure Data Factory (ADF), Azure Databricks (ADB), and Azure SQL Database, to create a robust pipeline for handling and visualizing COVID-19 data streams.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Data Sources](#data-sources)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Acknowledgements](#acknowledgements)

## Features
- **Data Ingestion**: Use Azure Data Factory to ingest COVID-19 data from various sources.
- **Data Processing**: Leverage Azure Databricks for data cleaning, transformation, and analysis.
- **Data Storage**: Store processed data in Azure SQL Database for querying and visualization.
- **Real-Time Analytics**: Enable real-time analytics and reporting through Power BI integration.

## Architecture
The project follows a typical data engineering architecture:
1. **Data Ingestion**: ADF pipelines extract data from online sources.
2. **Data Storage**: Raw data is stored in Azure Data Lake Storage (ADLS).
3. **Data Processing**: Databricks notebooks process and transform the data.
4. **Data Storage**: Processed data is loaded into Azure SQL Database.
5. **Data Visualization**: Power BI dashboards provide real-time insights.

## Data Sources
The project uses the following data sources:
- **COVID-19 Data**: Daily updates on COVID-19 cases, deaths, and recoveries in the UK.
  - Source: [Public Health England](https://github.com/MisraSwarup45/BritCovid_DataStream)
- **Demographic Data**: Population data to understand the impact across different regions.
  - Source: [Office for National Statistics](https://github.com/MisraSwarup45/BritCovid_DataStream)

## Setup and Installation
To set up and run this project, follow these steps:

### Prerequisites
- Azure Subscription
- Azure Data Factory
- Azure Databricks
- Azure SQL Database

### Steps
1. **Clone the repository**
   ```bash
   git clone https://github.com/MisraSwarup45/BritCovid_DataStream.git
   cd BritCovid_DataStream
   ```

2. **Set up Azure Data Factory**
   - Create ADF instance and import the provided pipelines.
   - Configure the linked services for data sources and sinks.

3. **Set up Azure Databricks**
   - Create a Databricks workspace.
   - Import the provided notebooks and configure them.

4. **Set up Azure SQL Database**
   - Create an Azure SQL Database instance.
   - Execute the provided SQL scripts to create necessary tables and schemas.

## Usage
1. **Run the ADF pipelines** to ingest the data.
2. **Execute Databricks notebooks** to process and transform the data.
3. **Load the processed data** into Azure SQL Database.

## Acknowledgements
- **Public Health England** for providing COVID-19 data.
- **Office for National Statistics** for demographic data.
- Azure for providing cloud infrastructure.
